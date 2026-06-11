**PsySuite build guide**<br>
<br>

PsySuite is a modular App, with an Application Module embedding four library modules.<br>
To build its APK, you need to pull the code from the following repository:<br>

**[psysuite](https://github.com/psysuite/psysuite)**: Is the Application module, implementing the dynamic menu and managing settings, projects and results submission.<br>
User must checkout the *demo_paper2* branch, that points to the library containing the tests of the demo version

**[psysuitecore](https://github.com/psysuite/psysuitecore)**: This library module is the project's common framework, defining all the common resources and superclasses that each concrete task will override. To playback auditory stimuli, it uses an aar file that implements sound playback mechanisms using Oboe (https://github.com/google/oboe).<br>
The source repository generating such file can be found here: https://github.com/albaspazio/nativeaudio

**[psysuitests-demo](https://github.com/psysuite/psysuitetests-demo)**: This library module contains the implemented Tasks.

**[psysuitepython](https://github.com/psysuite/psysuitepython)**:  This library module interacts with the python engine to access the primitives defined in ADOpy package.  

**[core](https://github.com/albaspazio/android-core)**:  This library module is a multi-purpose library of utilities methods.<br>

<br>
Modules are accessed by psysuite using a relative path organization. 
By default, at the level of the folder where you download psysuite repo, you should create a "modules" folder containing the four library modules codebase. <br>
<br>

- psysuite root  
- modules  
    |  
    |__  psysuitecore  
    |  
    |__  psysuitetests_demo2  
    |  
    |__  psysuitepython  
    |  
    |__  core  

**API Key**<br>

The app submits task results to a remote server and requires an API key and server URL that are not included in the repository.<br>
To test submission, create the file local.properties in the psysuite root and add the following entries:<br>

PSYSUITE_API_URL_RELEASE=https://your-server.com/api<br>
PSYSUITE_API_KEY_RELEASE=your-api-key<br>

Contact the repository maintainer (name.surname _at_ gmail.com) to obtain the values for these fields.<br>

**Release Signing**<br>

Release builds require a keystore and credentials that are not included in this repository.<br>
To simply test the app, you can build a debug version.<br>
If you want a release version, Create a .signing/ folder in the psysuite root containing:<br>

psysuite_keystore.jks — the keystore file<br>

password.properties — with the following keys:<br>
* keyAlias=your_key_alias<br>
* storePassword=your_store_password<br>
* keyPassword=your_key_password<br>

Contact the repository maintainer to obtain these files.<br>
If password.properties is not found, the build will automatically fall back to the debug signing config, which is sufficient for local testing.

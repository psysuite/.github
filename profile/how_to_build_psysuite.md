**PsySuite build guide**<br>
<br>

PsySuite is a modular App, with an Application Module embedding four library modules.<br>
To build its APK, you need to pull the code from the following repository:<br>

**[psysuite](https://github.com/psysuite/psysuite)**

Is the Application module, implementing the dynamic menu and managing settings, projects and results submission.<br>
User must checkout the *demo_paper2* branch, that points to the library containing the tests of the demo version

**[psysuitecore](https://github.com/psysuite/psysuitecore)**

This library module is the project's common framework, defining all the common resources and superclasses that each concrete task will override.<br>
To playback auditory stimuli, it uses an aar file that implements sound playback mechanisms using Oboe (https://github.com/google/oboe).<br>
The source repository generating such file can be found here: https://github.com/albaspazio/nativeaudio

**[psysuitests-demo](https://github.com/psysuite/psysuitetests-demo)**

This library module contains the implemented Tasks.

**[psysuitepython](https://github.com/psysuite/psysuitepython)**

This library module interacts with the python engine to access the primitives defined in ADOpy package.  

**[core](https://github.com/albaspazio/android-core)**

This library module is a multi-purpose library of utilities methods.<br>


Modules are accessed by psysuite using a relative path organization. 
By default, at the level of the folder where you download psysuite repo, you should create a "modules" folder containing the four library modules codebase. <br>

- psysuite root  
- modules  
    |  
    |_ psysuitecore  
    |  
    |_ psysuitetests_demo2  
    |  
    |_ psysuitepython  
    |  
    |_ core  


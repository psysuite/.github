This is the official repository of PsySuite project, a smartphone-based framework for implementing psychophysical testing on Android devices.<br>

The project was coded by Alberto Inuggi, biomedical engineer and Ph.D in experimental neurology<br>
It was started when he was enrolled in the U-VIP laboratory, headed by Dott.sa Monica Gori in the Istituto Italiano di Tecnologia of Genoa.<br>
The current 2.x version results from complete architectural redesign, refactoring, and development of new features performed when he moved to IRCCS Azienda Ospedaliera Metropolitana of Genova.

PsySuite embed the following features:

- run psychophisics tasks by delivering multisensory (auditory, visual and tactile) stimuli. 
- it contains a set of sensorial and cognitive tasks, exploring different domains.
- speech recognition allows blind users to run auditory and tactile tasks.<br>

from version 2.x.x:

- stimuli intensities are defined at run-time according to user responses, according to an adaptive design optimization (ADO) mechanism.
- can send experiment results to a web application that allow researchers to access and download the uploaded data
<br>

Version 1.x.x of the project was validated here: https://link.springer.com/article/10.3758/s13428-024-02475-4<br>
Version 2.x.x has been recently submitted

Presently, guest users can access a demo version of PsySuite shipped with three tasks:<br>
- reaction times
- temporal bisection task (discriminating stimuli' onsets rather than durations) 
- double flash illusion test

You can download its APK [here](https://github.com/psysuite/psysuite/releases/download/DEMO_RELEASE/app-demo.apk)

Otherwise you can pull all the necessary repositories, distributed with [Apache 2.0 Licence](https://github.com/psysuite/.github/blob/main/profile/LICENCE), and build PsySuite on your own.<br>
Please, read the [instructions](https://github.com/psysuite/.github/blob/main/profile/how_to_build_psysuite.md) 


**Collaborations**<br>

Upon specific request to psysuite _at_ gmail.com, it is possible to have access to further tasks.<br>
I'm also open to develop new tasks

These are the tasks already implemented<br>

*temporal domain*

- Temporal Bisection
- Temporal interval discrimination
- Temporal binding
- Temporal Interval reproduction

*prediction*

- temporal Sequence prediction
- Time-to-contact

*illusions*

- Double/Triple flash illusion
- figure/ground illusion
- ocular rivalry/grouping

*Miscellaneous*

- Reaction Times
- Beads test
- Musical Meters Discrimination task
 

**External references**<br>

- ADO algorithms are implemented using the ADOpy package, a python package described in the work of https://doi.org/10.3758/s13428-020-01386-4 whom code can be found here: https://github.com/adopy/adopy.<br>
- Python engine, necessary to execute ADOpy code, was embedded in Android thanks to the Chaquopy SDK (https://chaquo.com/chaquopy)

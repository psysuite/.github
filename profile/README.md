This is the official repository of PsySuite project, a smartphone-based framework for implementing psychophysical testing on Android devices. 
The project was entirely coded by Alberto Inuggi, biomedical engineer and Ph.D in experimental neurology 
It was started when he was enrolled in the U-VIP laboratory, headed by Dott.sa Monica Gori in the Istituto Italiano di Tecnologia of Genoa. 
The project was further improved when he moved to IRCCS Ospedale San Martino of Genoa, reaching now the version 2.x.x. PsySuite embed the following features:

- run psychophisics tasks by delivering multisensory (auditory, visual and tactile) stimuli 
- stimuli intensities are now (since version 2.x.x) defined at run-time according to user responses following an adaptive design optimization (ADO) mechanism 
- it contains a set of cognitive tasks, mainly exploring temporal domains: 
- an acoustic user interface, based on speech recognition, allow blind users to run part of the tasks implemented 
- Since version 2.x.x, can send experiment results to a web application that allow researchers to access and download the uploaded data

Version 1.x.x of the project was validated here: https://link.springer.com/article/10.3758/s13428-024-02475-4 
Version 2.x.x has been recently submitted

Tasks currently implemented

temporal domain

Temporal Bisection
Temporal interval discrimination
Temporal binding
Temporal Interval reproduction
prediction

temporal Sequence prediction
Time-to-contact
and illusions

Double/Triple flash illusion
figure/ground illusion
External references ADO algorithms are granted by ADOpy package, a python package described in the work of https://doi.org/10.3758/s13428-020-01386-4 whom code can be found here: https://github.com/adopy/adopy Python engine, necessary to execute ADOpy code, was embedded in Android thanks to the Chaquopy SDK (https://chaquo.com/chaquopy)

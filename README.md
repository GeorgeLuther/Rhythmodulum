# Rhythmodulum
A web application for generating and manipulating rhythmic patterns.

Right now I am working on a new version. My main goals for this are version are:
*Use a class/method solution for pattern functions and storage
*Interact more dynamically with the DOM
*Approach the audio playback more efficiently (revisit the way clocking and loading work)
*Add more drums and the ability to upload samples.
*Add MIDI clock and MIDI OUT functionality (working on a technique that can be similarly applied to my choralator project.

##Related documents
*[Brainstorming Page](https://docs.google.com/document/d/1qna9LV6pVFz6dmoLarC0cDfFT0yUagPQ5ojL8ECmYhE/edit?usp=sharing)
*[Pseudo-code](https://docs.google.com/document/d/1_Gs1Dd85kNEGzAkxlfWniV9NHmvzL31Z9DyOsfgEEDA/edit?usp=sharing)
*[UI Sketching](https://docs.google.com/presentation/d/12ZCTV_D56bZNKkaJkFE0Ulknrr_kYX3Gdpy_WH7OXes/edit?usp=sharing)

##Current functionality
* 8 drum sounds
* a basic transport bar
*'unlimited' patterns that can be named, sorted, and deleted
*individual play/pause button
*13 pattern generation/manipulation tools

##Pattern Generation/Manipulation Techniques:
*pulse - triggers on every beat of the bar
*beat - triggers on a specific beat (allows negative numbers)
*periodic - triggers on every Xth beat regardless of the bar length
trigger every ? beats
*cyclic - triggers on every Xth beat but resets each bar
trigger every ? beats
*subdivision - triggers are dispersed at a division of the bar length
divide bar by ?
*even - a chosen number of triggers are dispersed as evenly as possible throughout the bar
trigger on ? beats
*first - a chosen number of triggers fill from the beginning of the bar
trigger on ? beats
*last - a chosen number of triggers fill from the end of the bar
trigger on ? beats
*random - a chosen number of triggers are dispersed randomly throughout the bar
trigger on ? beats
*opposite - all rests become triggers, all triggers become rests.
I.E. 0,0,1,0,1 becomes 1,1,0,1,0 
*reverse - the existing bar is flipped
I.E. 0,0,1 becomes 1,0,0
*rotation - the existing bar is rotated by X beats
 	I.E. 1,0,0 becomes 0,1,0 (accepts negative numbers
rotate by ? beats
*grab - clones another rhythm’s current pattern (ALMOST FINISHED IN NEW VERSION)


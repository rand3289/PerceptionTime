## Modeling and reasoning about information transfer in biological and artificial organisms.

This is a summary/extension of my paper "Perception and Time in AGI".  

Computers and brains work in different ways.  Computers operate on symbols where as brains perceive the environment.  Communication using symbols and perception both describe information flow.  Below I try to state the differences between the two approaches.

One way of learning about any system is to divide it into parts and study interactions among the parts.  To model information flow in organisms they can be thought of as collections of observers receiving information from the outside world and performing actions.  A neuron is one example of an observer.

Observation is a mechanism where processes in the world (everything outside of a single observer) change that observer.  There are many mechanisms of change.  What changes within the observer is called "internal state".  Internal state is delimited from the world by a boundary that defines the observer.  The boundaries can change over time, overlap or contain one another.  Information travels across the boundaries via numerous mechanisms that change the internal state.  In non-virtual environments "internal state" is equivalent to "thermodynamic state" of the observer.  In other words, state can describe matter in the real world or bits in a virtual system.  

https://en.wikipedia.org/wiki/Thermodynamic_state  

When processes originating in the world change the observer, the observer detects this change.  The change is not "measured" in any way.  It is detected.  Detection is followed by an action that possibly changes other observers.  Detection is any mechanism that causes an action.  There is only ONE action for any one observer. Just like there is only one way for a neuron to fire.  However since an action is an interaction with the environment, its properties can be affected by the environment.  

Detection is best described by when the change has occurred.  This time instance can be represented as a point on a time line.  This type of description leads to a mathematical model called a Point Process.

Coincidence detection mechanism in neurons can help explain detection mechanism described above.  In my theory however, instead of detecting input signals, a change in the internal state (membrane potentialof a neuron), caused by one or more inputs (perhaps neurotransmitters binding to synapses), is detected.  There are many mechanisms of change.  Photons, electrons, heat transfer, vibrations, pressure can all cause an internal state change.  By abstracting away from these mechanisms, we can create a simple model.  This model can be applied to real world systems or simulations.  

https://en.wikipedia.org/wiki/Coincidence_detection_in_neurobiology  

### Detection
The difficult problems is explaining why **detection** is the primary mechanism of information processing.  In my theory various mechanisms of change decouple observers.  There is no communication that takes place.  The purpose of **detection** is to initiate an action in the world that will possibly change internal state of other observers.  

This still does not answer why use detection to produce an action.  One could say that measuring the change in internal state can produce an action proportionate to the measure.  However a measure is a much more complex mechanism possibly requiring a timing mechanism.  Another problem is measuring involves delaying the action.  An action has to be delayed to measure different amounts of state change.  With state change detection, there is no delay.  

Measurements are operations performed on two or more events.  A measurement is one of **many** possible operations that can be performed on these events.  In other words two or more events can be interpreted differently to produce many different measurements.  By deciding to operate on measurements a system designer discards a lot of available information because other measurements can be made on the same events.  For example event count per unit of time or average time between events etc...  To get a better understanding on the subject, take a look at the event camera.  

https://en.wikipedia.org/wiki/Event_camera  

Systems that use information theory for modeling communication among "observers/agents/modules" suffer from a serious problem.  Measurements in the form of numbers, levels or symbols are inherently meaningless to other observers.  Observers have to agree on the symbols used for communication prior to communication taking place.  One can argue that they can be learned.  However you can't always agree on a set of symbols with your environment since processes in your environment can change.  Novel processes can appear at any time.  

### Examples
Detection/action mechanism is frequently found in biology in the form of a spike.  Artificial spiking neural networks try to model this behavior.  Researchers claim that SNNs are computationally and energy efficient often missing the point that detection should be treated as the main mechanism for computation.  If my theory is correct, we should put more effort in researching spiking ANNs.  

In electronics a comparator is an example of a detector.  Flash ADCs use a row of comparators that detect changes in their input to convert voltage levels into numbers.  The problem is they also perform sampling.  During sampling only one comparator which detected a change is selected per unit of time.  An ADC output value is an index of that comparator.  The precise time of detection by the selected comparator is lost.  Only a time interval is known.  If sampling frequency is below Nyquist frequency, detections by other comparators are also lost.  

https://en.wikipedia.org/wiki/Comparator  
https://en.wikipedia.org/wiki/Flash_ADC  
https://en.wikipedia.org/wiki/Sampling_(signal_processing)  
https://en.wikipedia.org/wiki/Nyquist_frequency  

### Implications
I call this mechanism "perception".  There is a lot of controversy around using the word perception.  However it can model the transformation that takes place on the boundary of our bodies as well as information flow deep inside our brains far from sensory neurons.  My goal is to make detection mechanism a standard tool in modeling AI systems. In addition, semantics or meaning can be reasoned about by specifying that an internal change is meaningful for an individual observer.  


toandrey(at)yahoo(dot)com  
document created April 30, 2021  
last modified May 8, 2022  

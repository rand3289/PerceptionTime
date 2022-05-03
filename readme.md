## Modeling and reasoning about information transfer in biological and artificial organisms.

This is a summary/extension of my paper "Perception and Time in AGI".  

Computers and brains work in different ways.  Computers operate on symbols where as brains perceive the environment.  Communication using symbols and perception both describe information flow.  Below I try to state the differences between the two approaches.

One way of learning about any system is to divide it into parts and study interactions among the parts.  To model information flow in organisms they can be thought of as collections of observers receiving information from the outside world and performing actions.  A neuron is one example of an observer.

Observation is a mechanism where processes in the world (everything outside of a single observer) change that observer.  There are many mechanisms of change.  What changes within the observer is called "internal state".  Internal state is delimited from the world by a boundary that defines the observer.  The boundaries can change over time, overlap or contain one another.  Information travels across the boundaries via numerous mechanisms that change the internal state.  In non-virtual environments "internal state" is equivalent to "thermodynamic state" of the observer.  In other words, state can describe matter in the real world or bits in a virtual system.  

https://en.wikipedia.org/wiki/Thermodynamic_state  

When processes originating in the world change the observer, the observer detects this change.  The change is not "measured" in any way.  It is detected.  Detection is followed by an action that possibly changes other observers.  Detection is any mechanism that causes an action.  There is only ONE action for any one observer. Just like there is only one way for a neuron to fire.  However since an action is an interaction with the environment, its properties can be affected by the environment.  

Detection is best described by when the change has occurred.  This time instance can be represented as a point on a time line.  This type of description leads to a mathematical model called a Point Process.

Coincidence detection mechanism in neurons (https://en.wikipedia.org/wiki/Coincidence_detection_in_neurobiology) can help explain detection mechanism described above.  In my theory however, instead of detecting input signals, a change in the internal state (membrane potentialof a neuron), caused by one or more inputs (perhaps a neurotransmitter binding to a synapse), is detected.  There are many mechanisms of change.  Photons, electrons, heat transfer, vibrations, pressure can all cause an internal state change.  By abstracting away from these mechanisms, we can create a simple model.  This model can be applied to real world systems or simulations.  

### Detection
I consider most of the statements above obvious.  Please email me if you disagree.  The difficult problems is to explain why DETECTION is the primary mechanism of information processing.  Systems that use information theory by modeling communication among "observers/agents/modules" suffer from a serious problem I describe below.  In my theory various mechanisms of change decouple observers.  There is no communication that takes place.

The purpose of DETECTION is to initiate an action in the world that will possibly change internal state of other observers.  This still does not answer why use detection to produce an action.  One could say that measuring the change in internal state can produce an action proportionate to the measure.  However a measure is a much more complex mechanism possibly involving an oscillator for timing.  Another problem is measuring involves delaying the action.  An action has to be delayed to measure different amounts of state change.  With state change detection, there is no delay.  

Measurements are operations performed on two or more events.  A measurement is one of **MANY** possible operations that can be performed on these events.  In other words two or more events can be interpreted differently to produce many different measurements.  To get a better understanding on the subject, take a look at the event camera. (https://en.wikipedia.org/wiki/Event_camera)  By deciding to operate on measurements a system designer discards a lot of available information because other measurements can be made on the same events.  For example event count per unit of time or average time between events etc...

Measurements in the form of numbers are useless to other observers because that would imply there is communication taking place among observers.  The problem faced by systems where modules/agents/observers communicate is that observers have to agree on the mechanisms used for communication.  Symbols, numbers or levels used for communication have to be known prior to communication taking place.  One can argue that they can be learned by observers.  However you can't agree on a set of symbols with your environment since processes in the environment continue to change.  Novel processes can appear any time.  This statement assumes interactions among observers and interactions of observers with their environment should be modeled the same way.

This question can be stated differently: why wouldn’t an agent/observer generate information in the form of a spike?  One possibility it performs a measurement which we discussed above.  Another possibility is that it performs detection of categories.  In this case the solution is also simple: treat different categories as individual observers.

### Implications
* My goal is to make this mechanism a standard tool in developing AI systems.  Justifying why spiking ANNs is the way to go.
* I call the mechanism "perception".  There is a lot of controversy around using the word perception.  However it can model the transformation that takes place on the boundary of our bodies as well as information flow deep inside our brains far from sensory neurons.
* It can be reasoned that detection mechanism is one of the signatures of life. The other being ability to reproduce.
* Semantics or meaning can be reasoned about by specifying that a change is meaningful for an individual observer only.
* Since time is just another property of the observation, it should be treated as a sensory modality.  For example an eye can register location, color, brightness and time of an observation for a given feature.

toandrey(at)yahoo(dot)com  
document created April 30, 2021  
last modified Nov 9, 2021  

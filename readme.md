## Modeling and reasonging about information transfer in biological and artificial organisms.

This is a summary of my paper "Perception and Time in AGI".

Embodiment is important for achieving Artificial General Intelligence.  It allows an embodied agent to conduct statistical experiments as opposed to simple observations.  If you subscribe to this proposition, the notion of data goes out of the window since all information has to be perceived by an embodied agent.  

One way of learning about any system is to divide it into parts and study interactions among the parts.  To model information flow in organisms they can be thought of as collections of observers or agents receiving information from the outside world and "transmitting information" from one observer to another.  In my theory I use words "change" and "action" instead of "receiving information" and "transmitting information".  This is a fundamental difference.  A neuron is an example of an observer.  

Observation of processes in the world (everything outside of a single observer including other observers) changes that observer.  There are many mechanisms of change.  What changes within the observer is called "internal state".  State can be matter in the real world observers or bits in artificial ones.  Internal state is dilimited from the world by a boundary that defines the observer.  The boundaries can change over time, overlap or contain one another.  Information travels across the boundaries via numerous mechanisms that change the internal state.  

When processes originating in the world change the observer, the observer detects this change.  The change is not "measured" in any way.  It is detected.  Detection is followed by an action that possibly changes other observers.  Detection is any mechanism that causes an action.  There is only ONE action for any one observer.  It remains a question if the action can be affected by the internal state.  However it is my belief the action does NOT vary in force or duration or information that can be gathered about it from an observer's perspective.  However since an action is an interaction with the environment, its properties are affected by the environment.  

Detection is best described by when the change occured.  This time instance can be represented as a point on a time line.  This type of description leads to a mathematical model called a Point Process.

Coincidence detection mechanism in neurons (https://en.wikipedia.org/wiki/Coincidence_detection_in_neurobiology) can help explain detection mechanism described above.  In my theory however, instead of detecting input signals, a change in the internal state (membrane potential), caused by ONE or more input signals, is detected.

State change takes place in things dead or alive.  However only live observers can detect changes.  Other clumps of matter change their internal state but rearly detect changes.  (There are exceptions like thermostats.)  There are many mechanisms of change.  Photons, electrons, heat transfer, vibrations, pressure can all cause an internal state change.  By abstracting away from these mechanisms of change, we can create a simple model.  This model can be applied to the real world or a simulation.

### Detection
I consider most of the statements above obvious.  Please email me if you disagree.  The difficult problems is to explain why DETECTION is the primary mechanism of information processing.  Anything that uses communication among "observers/agents/modules" suffers from a serious problem I describe below.  In my theory various mechanisms of change decouple observers.  There is no COMMUNICATION that takes place.

The purpose of DETECTION is to initiate an action in the world that will possibly change internal state of other observers.  This still does not answer why use detection to produce an action.  One could say that measuring the change in internal state can produce an action proportionate to the measure.  However a measure is a much more complex mechanism possibly involving an oscillator for timing.  Another problem is measuring involves delaying the action.  An action has to be delayed to measure different amounts of state change.  With state change detection, there is no delay.  

Measurements are operations performed on two or more events.  A measurement is one of MANY possible operations that can be performed on these events.  In other words two or more events can be interpreted differently to produce many different measurements.  To get a better understanding on the subject, take a look at the event camera. (https://en.wikipedia.org/wiki/Event_camera)  By deciding to operate on measurements a system designer discards a lot of available information because other measurements can be made on the same events.  For example event cound per unit of time or average time between events etc...

On the other side biological neurons can be said to operate on events and produce measurements.  However this is a measurement a neuron choses to make.  Value is not supplied from an outside.  The result of the measurement is a spike.  Following this logic, there should be a reduction in the number of spikes up the chain since it takes at least two events (spikes from other observers) to make a measurement.

Measurements in the form of numbers are useless to other observers because that would imply there is communication taking place among observers.  The problem faced by systems where modules/agents/observers communicate is that observers have to agree on the mechanisms used for communication.  Symbols, numbers or levels used for communication have to be known prior to communication taking place.  One can argue that they can be learned by observers.  However you can't agree on a set of symbols with your environment since processes in the environment continue to change.  This statement assumes interaction among observers and interaction of observers with their environment should be modeled the same way.


### Implications
* My goal is to make this mechanism a standard tool in developing AI systems.  Justifying why spiking ANNs is the way to go.
* I call the mechanism "perception".  There is a lot of controversy around using the word perception.  However it can model the transformation that takes place on the boundary of our bodies as well as information flow deep inside our brains far from sensory neurons.
* It can be reasoned that detection mechanism is one of the signatures of life. The other being ability to reproduce.
* Symantics or meaning can be reasoned about by specifying that a change is meaningful for a single observer only.


toandrey(at)yahoo(dot)com  
document created April 30, 2021
last modified Oct 26, 2021
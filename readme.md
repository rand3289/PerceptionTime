## TLDR
We propose the following abstraction to help think about perception from a point of view of a system operating in an environment.  The system is composed of multiple agents. There are various processes occurring in the environment. An agent can become part of a process.  This results in the process (environment) modifying internal state of an agent.  When this occurs, we say information crosses the boundary between an agent and a process.  The agent can then detect this change within self. Making each agent a change detector.  This change is best described by the time at which it has occurred.  This way all information that crosses the boundary is expressed as points in a continuous time domain.  The agents self-organize within the system to figure out what type of changes they detect.  

## Summary
Artificial General Intelligence (AGI) implies a system capable of sensing and manipulating any environment.  The way the environment is sensed has to be independent from the modality and dimentionality of the environment itself.  This transformation has to take place on the border of a system and its environment.  Hence the notion of a boundary between an agent and its environment becomes essential.  

Current algorithms work on symbols/numbers/tokens which are created by measuring things in the environment.  The problem with measurements is that you need to know exactly what you are measuring. You create an assumption that what you are measuring gives you enough relevant information about the environment.  In reality the step of measuring the environment is not necessary.  Measurements are artifacts left over from human habbit of making measurements to record and convey information.  

The way any biological or artificial sensor works is the environment modifies the internal state of the sensor.  For example photons hitting a retina or a CCD sensor.  At this point what happens in most current artificial sensors is a measurement is made.  For example a count of photons hitting a pixel is taken over a period of time (exposure time).  On the other side, most biological sensor do not make a measurement.  They detect a change within itself and signal the fact that the change was detected to other parts of the system / agents.  For example a retinal neuron detects that the membrane potential has changed and fires.  Some artificial sensors such as event cameras exibit similar behavior.  

The fact of detecting a change is called perception.  The reason this is called perception and not just sensing is that other parts of the system can affect how that neuron detects a change within itself.  Perception is a subjective experience since the change is detected within self.  Detection mechanism represents information in terms of points on a time line.  These points represent when a change was detected.  

## Important distinction
Notice how a CCD sensor counted how many photons hit the pixel during a period of time.  It performed an integration operation on the signal. From the point of view of current artificial sensors, biological sensors operate on derivatives (instantaneous changes).  

## Modeling and reasoning about information transfer in biological and artificial organisms.

The rest of this article provides a description of a tool for thinking about information processing. It is also a summary/extension of my paper "Perception and Time in AGI".  

Computers and brains work in different ways.  Computers operate on symbols where as brains perceive the environment.  Communication using symbols and perception both describe information flow.  Below I try to state the differences between the two approaches.  

One way of learning about any system is to divide it into parts and study interactions among the parts.  
Parts within a computer use bits to share information.  A bit is never just 1 or 0. A bit has a value of one or zero on some interval of time.  It can change its value at some point in time.  Conventional neural networks (NNs) operate on bits whereas biological and artificial spiking NNs operate on spikes (points in time when a change occurs).
To model information flow in organisms they can be thought of as collections of observers receiving information from the outside world and performing actions.  A neuron is one example of an observer.  

Observation is a mechanism where processes in the world (everything outside of a single observer) change that observer.  There are many mechanisms of change.  What changes within the observer is called "internal state".  Internal state is delimited from the world by a boundary that defines the observer.  The boundaries can change over time, overlap or contain one another.  Information travels across the boundaries via numerous mechanisms that change the internal state.  In non-virtual environments "internal state" is equivalent to "thermodynamic state" of the observer.  In other words, state can describe matter in the real world or bits in a virtual system.  

https://en.wikipedia.org/wiki/Thermodynamic_state  

When processes originating in the world change the observer, the observer detects this change.  The change is not "measured" in any way.  It is detected.  Detection is followed by an action that possibly changes other observers.  Detection is any mechanism that causes an action.  There is only ONE action for any one observer. Just like there is only one way for a neuron to fire.  However since an action is an interaction with the environment, its properties can be affected by the environment.  

Detection is best described by when the change has occurred.  This time instance can be represented as a point on a time line.  This type of description leads to a mathematical model called a Point Process.

Coincidence detection mechanism in neurons can help explain detection mechanism described above.  In my theory however, instead of detecting input signals, a change in the internal state (membrane potential of a neuron), caused by one or more inputs (perhaps neurotransmitters binding to synapses), is detected.  There are many mechanisms of change.  Photons, electrons, heat transfer, vibrations, pressure can all cause an internal state change.  By abstracting away from these mechanisms, we can create a simple model.  This model can be applied to real world systems or simulations.  

https://en.wikipedia.org/wiki/Coincidence_detection_in_neurobiology  

### Detection
The difficult problems is explaining why **detection** is the primary mechanism of information processing.  In my theory various mechanisms of change decouple observers.  There is no communication that takes place.  The purpose of **detection** is to initiate an action in the world that will possibly change internal state of other observers.  

This still does not answer why use detection to produce an action.  One could argue that measuring the change in internal state can produce an action proportionate to the measure.  However a measure is a much more complex mechanism possibly requiring a timing mechanism.  Another problem is measuring involves delaying the action.  An action has to be delayed to measure different amounts of state change per interval of time.  With state change detection, there is no delay.  

Measurements are operations performed on two or more events.  A measurement is one of **many** possible operations that can be performed on these events.  In other words two or more events can be interpreted differently to produce many different measurements.  By deciding to operate on measurements a system designer discards a lot of available information because other measurements can be made on the same events.  For example event count per unit of time or average time between events etc...  To get a better understanding on the subject, take a look at the event camera.  

https://en.wikipedia.org/wiki/Event_camera  

In electronics a comparator is an example of a detector.  Flash ADCs use a row of comparators that detect changes in their input to convert voltage levels into numbers.  The problem is they also perform sampling.  During sampling only one comparator which detected a change is selected per unit of time.  An ADC output value is an index of that comparator.  The precise time of detection by the selected comparator is lost.  Only a time interval is known.  If sampling frequency is below Nyquist frequency, detections by other comparators are also lost.  

https://en.wikipedia.org/wiki/Comparator  
https://en.wikipedia.org/wiki/Flash_ADC  
https://en.wikipedia.org/wiki/Sampling_(signal_processing)  
https://en.wikipedia.org/wiki/Nyquist_frequency  

Systems that use information theory for modeling communication among "observers/agents/modules" suffer from a serious problem.  Measurements in the form of numbers, levels or symbols are inherently meaningless to other observers.  Observers have to agree on the symbols used for communication prior to communication taking place.  One can argue that they can be learned.  However you can't always agree on a set of symbols with your environment since processes in your environment can change.  Novel processes can appear at any time.  Information theory requires a receiver to have some knowledge about a transmitter.  For example to determine an appropriate Nyquist frequency or if the signal is generated by a stationary process.  

### Mechanisms of change
There are various mechanisms that can change the internal state of the observer. Ironically some can be described in terms of symbols. One can argue that biological systems use neurotransmitters as symbols and the meaning of these symbols have been shared through DNA according to which the cells built the ion channels. This description however can NOT be applied to the perception mechanism applicable on the border of the organism and its environment.  

### Implications
Is there a fundamental difference between computing models used in digital computers and biology?  In digital systems subsets of bits change their values synchronously at a point in time usually upon a central clock edge transition.  On the other hand detection/action mechanism is frequently found in biology in the form of a spike.  

Artificial spiking neural networks try to model this behavior.  Researchers claiming that SNNs are simply computationally and energy efficient miss the point that detection should be treated as the main mechanism for computation.  

I call this detection mechanism "perception".  There is a lot of controversy around using the word perception.  However it can model the transformation that takes place on the boundary of our bodies as well as information flow deep inside our brains far from sensory neurons.  My goal is to make detection mechanism a standard tool in modeling AI systems. In addition, semantics or meaning can be reasoned about by specifying that an internal change is meaningful only for an individual observer and therefore it is an underlying mechanism for qualia.  

## A statistical experiment
Information extracted by measuring can not represent all possible environments well.  Imagine you have a statistical experiment in which you throw a fair six sided die. Let's say the experiment was repeated three times. You can model this in two ways:  

As a stochastic proces with a discrete RV representing the number of dots on a die or as a two dimentional temporal point process with a discrete number of dots on y axis and continuous time on x axis.  

You can argue that these models are identical, but this is simply not true when dealing with the real world. In the real world a die can land on something half way and produce an undetermined result or be obscured by some object. First model will not be able to represent an outcome in its statespace. Second model will simply have two points instead of three.  

You might think oh, I will just modify the statespace in the first model, but it will work only until your kid throws a second die on the table modifying the experiment.  How do you represent state if the die gets covered by a piece of paper?  Should the internal representation of the environment stay the same?  

This is a simple toy example but I argue that unless you use temporal point processes your model will never create a good representation of a phenomenon in the real world.  Unless you use point processes, your statespace has to be able to represent all possible combinations of state of the environment. Which is impossible.  


## Conclusion
Our perception system maps senses from multiple modalities into a point in 3 dimentions of space plus time. Location of a neuron in 3D space plus when it fired.  Since the observers/agents/neurons which are part of our perception system have boundaries, we can enumerate them.  This reduces the dimentionality of the information to two dimentions.  One discrete and one continuous (time).  To describe a single point in multi-dimentional space one needs several numbers or symbols.  One for each dimention.  Therefore using a single symbol is not sufficient when trying to represent multi-modal information.  

When data is created, one of two hacks are used.  Information can be represented as a sequence completely devoid of timing information. Alternatively it can be represented as time series where time is represented in terms of discrete intervals.  When time series is created, information is integrated over a period of time.  This period of time is an arbitrary constant introduced by the designer of the system.  This transformation looses some information.  Furthermore the arbitrary period of time creates side effects.  One side effecct is described in Nyquist theorem.  

When creating a system, think of information in terms of points.  Not data!  Separate the ideas and implementation details.


toandrey(at)yahoo(dot)com  
document created April 30, 2021  
last updated June 10, 2025  


KERA README

Full documentation can be found in the pdf doc file and with the supplement of the NAR paper ()


KERA (Kinetic Event Resolving Algorithm) is a tool for analyzing data which consists of time-series of data at discrete states.  It was originally designed for use in single-molecule fluorescence studies.  In these, the fluorescence levels of individual molecules (visualized by TIRF microscopy or similar) are discretized through the use of a program such as QuB, HaMMY, or ebFRET.  The resulting discrete traces have a specified number of “states”.  However, in many fluorescence studies, multiple reporter molecules with distinguishable fluorescence are used (a common pair is Cy3 and Cy5, which are spectrally distinct).  When two or more reporters are at the same location on the slide and imaged simultaneously, they are said to be co-localized; generally, this means that the two reporters are giving information about the same chemical environment simultaneously.  An example of this occurring: Cy3 fluorescence might be used to report the conformation of an immobilized protein, while Cy5 fluorescence reports on the binding of a DNA molecule to the protein.  These distinct signals are referred to as channels within KERA.  KERA supports any number of channels, and any number of states within each channel.  The original conception of KERA was as an Excel macro which was designed to distinguish the possible configurations of a 2-channel, 2-state (each) system; this motivation is detailed in the thesis of Dr. Elizabeth Boehm and explored more in the 2016 review by Boehm et al.  From there, efforts have been made to make the interface more user-friendly, and to expand the capabilities of the program to encompass more complicated systems.  

KERA is not a discretization software; much more advanced work has been done to create robust methods of turning a noisy trace into discrete steps.  KERA is  solely meant to take in those discretized traces and organize them in a method which makes it easier to see the transitions, interactions between channels, and kinetics of the events contained within.  If you need help with discretizing your data in the first place, you’ll probably want advice from someone who runs the same types of experiment as you, since the method of discretization sometimes depends on what the data looks like.

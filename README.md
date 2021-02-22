# SoftwareDesignDoc

# Briefly summarize The Gaming Room client and their software requirements. Who was the client? What type of software did they want you to design?
For this software design document, the client was the Gaming Room and they wanted to take their Android-only game, Draw It or Lose It, and expand it to other platforms through a web-based application.  They wanted the software to be designed such that only one instance of a game could exist in memory at any given time, each game could have multiple teams, and each team could have multiple players.  They also wanted to maintain security of user accounts through a login requiring a unique username and password.


# What did you do particularly well in developing this documentation?
This document clearly describes the use of object-oriented programming using Java including descriptions of encapsulation and polymorphism.  The use of Java for this applicationn works well given that it will be a web-based application with cross-platform compatibility.

# What about the process of working through a design document did you find helpful when developing the code?
Referring to the software design document was helpful in terms of keeping the client's requirments in mind and having the reference to go back to while developing the code.  The most useful part of the document was the UML diagram.  This served as a quick reference for the required aspects of the code that needed to be created, including all instance variables and methods as well as whether those variables and methods should be created as public or private.  It also clearly defined how the classes should be created within the overall package.

# If you could choose one part of your work on these documents to revise, what would you pick? How would you improve it?
I would spend more time on the overall evaluation of the pros and cons of the different operating systems.  I think this part is important to making the best recommendation to the client.  I would start by asking more questions of the client to determine if they had any budget constraints or other considerations, such as knowledge of the different operating systems, that they would like to take into account in terms of picking the best operating system for the server and the client.  I would also ask more clarifying questions about the client's preference for development tools.

# How did you interpret the user’s needs and implement them into your software design? Why is it so important to consider the user’s needs when designing?
The user requirement for only having one instance of the game in memory at any given time was implemented using the singleton pattern, which meant setting the constructor for the game instance as private in Java.  The code also implemented requirements for unique identifiers for game, team, and user names by using an iterator pattern to search for existing entries of these variables to determine uniqueness.  The code was also written to allow a game to have multiple teams and teams to allow teams to have multiple players.  User accounts were managed through the Dropwizard framework in Java.

# How did you approach designing software? What techniques or strategies would you use in the future to analyze and design a similar software application?
First and foremost, designing software requires listening to the client and determing their needs for the finished product.  With the client's requirements in place, I would pursue the feasibility of those requirements within the client's restraints, such as time and budget, as well as any other restraints, including limits of operating systems and platforms and coding limitations.  I would then make a recommendation to the client and ensure that the design plan is consistent with the client's expectations.  Finally, I would write code to meet the specifications of the software design.

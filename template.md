

![PROLOG](https://lh3.googleusercontent.com/proxy/7MkZojcJySJnw7dqB2ir6kk8in9ldmTvX4N-mYwQJWZ7X-97Vowbf8oLduz5WMSnHNVrjrvUW1JyXUnWDjgAPT-i0kurkw)
# PROLOG
##### What is Prolog?
Prolog is a logic programming language that designed by Alain Colmerauer & Robert Kowalski.Prolog word comes from "PROgrammation en LOGique" word in French. It has important role in artificial intelligence. Unlike many other programming languages, Prolog is intended as a declarative programming language.Based on fairly advanced mathematical and logical theories. It is used for complex systems. In prolog, logic is expressed as relations (called as Facts and Rules).Formulation or Computation is carried out by running a query over these relations.
Prolog, with its structure suitable for logical and symbolic thinking, is a tool that helps people in the stages of developing the methods required for the definition and solution of the problem.Prolog codes are interpreted by one interpreter, the code line written is interpreted, the result is produced and passed to another. Different from other languages.For example if the command is success it returns true.

 

###### History of language:
The language was developed and implemented in Marseille, France, in 1972 by Alain Colmerauer with Philippe Roussel, based on Robert Kowalski's procedural interpretation of Horn clauses.The first Prolog compiler was credited to David Warren, at the University of Edinburgh which is expert on Artifical Intelligence. Most commercial implementations of Prolog now use this same Edinburgh Prolog syntax.

###### Influenced / Influenced by
Prolog influenced by -> Planner
Influenced -> CHR, Clojure, Datalog, Erlang, KL0, KL1, Mercury, Oz, Strand, Visual Prolog, XSB


###### Why was it invented?
Prolog was invented for implement a man-machine communication system in natural language. It can be said that Prolog was a child of successful marriage between natural language processing and automated theorem-proving. In 1970's, the idea of using a natural language like French for communicate directly with a computer was madness. But this was the basis of the project set up by Alain Colmerauer.

###### When/Why using Prolog?
Prolog widely used for natural language processing and Artifical Intelligence. It is using at:

- Build expert systems that solve complex problems without the help of humans (e.g. automatically planning, monitoring, controlling and troubleshooting complex systems)
- Build decision support systems that aid organizations in decision-making (e.g. decision systems for medical diagnoses)
- Online support service for customers, etc.

Why shall we use?
Because;
-  In Prolog, you can treat data as programs. You can read a Prolog expression from file and then execute it, or build it on the fly and then execute it. That flexibility can be very useful.
-  Prolog is interactive. It comes with a top-level interpreter: a command interface that you can type code at and get it executed immediately.
-  You can do functional programming in Prolog, by using a translator such as Grips. 
-  In Prolog, you can write logical specifications of searches and get them executed without recoding into some more primitive language. For example, I can write:

```sh
mortal(X) :- man(X).     % X is mortal if X is a man.
man(socrates).           % Socrates is a man.
```
```
?- mortal(socrates).    % Is Socrates mortal?
```
Then it will immediately say YES!. 

###### Prolog Environments
Prolog has too many environments like;
- GNU Prolog

This Prolog compiler complies with the ISO standard for Prolog (with useful extensions like global variables, ability to interface with the operating system, etc) Platforms supported include Linux (ix86 & PowerPC), Win32(ix86), FreeBSD, OpenBSD, NetBSD, Darwin (PowerPC), SunOS (sparc) and Solaris (ix86 & sparc).

- Open Prolog 

Open Prolog supports many features of ISO Prolog, including disjunctive calls, negation, if-then and if-then-else, program originated catch and throw exception handling etc.It runs on Apple Macintosh machines running Mac OS 7.5.5 and later, as well as under the Classic environment of Mac OS X.

- Ciao Prolog

Ciao Prolog is a GNU GPL Prolog system that supports ISO Prolog as well as various extensions, such as programming with functions, objects, threads, etc. Precompiled binaries are available for Windows, and the sources may be compiled for Linux, Mac OS X, SunOS, Solaris, IRIX, etc.

- Poplog

Poplog is a software development system that includes incremental compilers for Pop11 (a Lisp-like language with more conventional syntax), Common Lisp (compatible with CLTL2 - Common LISP: The Language, 2nd edition), Prolog (compatible with the Edinburgh definition), and Standard ML. It comes with documentation, program libraries, and teaching materials for AI and Cognitive Science. Supported platforms include Windows, Linux, Solaris on Sparc, Solaris on Intel, Digital Unix on Alpha, AIX on PowerPCs. The downside is that the windows support is limited to W95, W98 and NT.


- SWI Prolog 

SWI-Prolog supports Edinburgh Prolog and large parts of ISO Prolog. This system sports a robust compiler, a good set of built-in predicates and a flexible interface to the C and C++ language. SWI-Prolog is portable to many platforms, including most Unix/Linux platforms, Windows (NT/2000/XP) and MacOS X (using X11 for graphics). Both 32-bits and 64-bits hardware is supported. Both sources and binaries (Win32, almost all Unix platforms, etc) are provided. The downside is that it does not have a visual level debugger and that it is not very fast.


##### How to Setup SWI-Prolog?
###### Installation in Windows: 
https://www.swi-prolog.org/download/stable
Select edition and install by following installer instructions.
DONE!
###### Installation in Linux :
Add the ppa ppa:swi-prolog/stable to your system’s software sources:

```sh 
sudo add-apt-repository ppa:swi-prolog/stable
```

Afterwards, update the package information:
```sh 
sudo apt-get update
```

Opening terminal and text: 
```sh
sudo apt-get install swi-prolog
```

DONE!

![Imgur](https://i.imgur.com/12bY9WN.png)

###### Quick Start Linux
1. Write a prolog program as a text file with a .pl ending. For example, program.pl
2. Open a terminal (Ctrl+Alt+T) and navigate to the directory where you stored your program.
3. Open SWI-Prolog by invoking 
```sh
swipl.
```
4. In SWI-Prolog, type [program] to load the program, i.e. the file name in brackets, but without the ending.
5. In order to query the loaded program, type goals and watch the output.
6. Alternatively, you can also load the program by passing its name as a parameter to SWI-Prolog: 
```sh
swipl -s program.pl.
```
7. To exit SWI-Prolog, type 
```sh
halt.
```
###### Installation in MacOS :
Install Homebrew. Homebrew is a command-line package manager for Mac which makes it much more simple and straightforward to install all sorts of things from and on the command line. Then simply execute:
$ brew install swi-prolog

#### If we want to learn SWI-Prolog without installing anything
SWI-Prolog official website offers SWISH, an online service for experimenting with and sharing SWI-Prolog programs.

##### Interesting and specific things 
If you want to run the program codes together you have written, but not one by one, you should write this to a file and install it in the prolog interpreter. It will send you the result by using the contents of the file as a database.The knowledge base is very important in the prolog, the results are obtained from the data in this knowledge base.Rules are determined in the knowledge base and the flow of the program is arranged as desired.The relation of a defined rule with another rule is reported and when the query is made, the prolog uses them and sends the appropriate result to the user.Rules are created in logic, so the prolog is completely logic-based language.
The prolog has a structure called the Decision Engine to carry out these processes. With this engine, a logical solution is found for the problem solution and the problem is solved.
When writing programs in the prolog, the objects and the relationships between these objects are determined first. Prolog creates a structure called predicate logic using these objects. These objects are selected from the incoming query and the remaining query sentence is left as it is.Thus, both fast and purposeful results are obtained. It also supports the prolog list structure and this structure further strengthens the prolog language.Lists are very useful for problem solving.
Prolog was used heavily in the European Esprit programme and in Japan where it was used in building the ICOT Fifth Generation Computer Systems Initiative. The Japanese Government developed this project in an attempt to create intelligent computers. Prolog was a main player in these historical computing endeavours.
Computer Science programs across various universities require their students to learn the Prolog programming language, usually in a discrete math course, and that students generally find it to be a rather unpleasant experience.

One of the places where using prolog is a good choice: Zebra puzzle. It is also known as Einstein's Riddle and it is rumored (not proven!) to be first proposed by the great scientist Albert Einstein. Furthermore, it is rumored that only about 2% of the world's population can solve this riddle correctly.I can explain this with a zebra puzzle example but it will be too long but if we examine the zebra puzzle we might have an idea.

###### Example codes
   woman(mia).
   woman(jody).
   woman(yolanda).
   playsAirGuitar(jody).
   party.

   ?-  woman(mia)
   
   prolog will answer : yes
Another Example:
sumlist([],0).
sumlist([H|T],N):-sumlist(T,N1),N is N1+H.

?- sumlist([1,2,3],N).

return N=6

Another example:
num[0].
num[1].
num[2].
num[3].
num[4].
num[5].
num[6].
num[7].
num[8].
num[9].
our_random(Lower,Upper,R):-
num(R ),
R >= Lower,
R <= Upper.

?-random(4,8,R).
 now it returns random integers between 4-8 also it can return 4 and 8.
Another Example:
reverse([],[]).
reverse(L1,R):-
L1=[H|T],
    reverse(T,R1),
    append(R1,[H],R).

?-reverse([3,2,1],R). 
 It returns R=[1,2,3]

###### Resources
https://www.mta.ca/~rrosebru/oldcourse/371199/prolog/history.html   
  https://www.sjsu.edu/faculty/watkins/prolog.html
http://alain.colmerauer.free.fr/alcol/ArchivesPublications/PrologHistory/19november92.pdf
  https://www.drdobbs.com/parallel/the-practical-application-of-prolog/184405220
https://www.swi-prolog.org/build/unix.html







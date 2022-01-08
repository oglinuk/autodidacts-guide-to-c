# History

If there was a modern example of the ancient Greek titan Atlas, it
would be the C programming language. The majority of phones run Linux,
which is written in C. The majority of web servers are running Nginx or
Apache, which are both written in C. Git, which is the most important
tool for versioning not just software, but data in general, is written in
C. There are plenty more examples of commonly used applications that are
written in C, which is a challenge for you to go and find at least two. A
good place to look is on GitHub. Before getting into C, it is important
to understand its history.

Back in the 1960s, Bell Labs (research and development department of AT&T
at the time) was involved in the development of a time-sharing operating
system called Multics, which was capable of running on different systems.
Among the people developing Multics were Dennis Ritchie and Ken Thompson.
In 1969 Bell Labs pulled out of the project, and in a famous story Ken
Thompson implemented the base for a new Unix system in 3 weeks while his
wife and daughter we on vacation. This was all done on a PDP-7. Unix and
C are as interconnected as Linux and Git. It is impotant to remember that
this is still before the creation of C.

Eventually Unix was ported to a PDP-11, which is around the time that the
famous Unix pipes and filters were created. Ken describes how he got the
idea for pipes from his supervisor at the time, Douglas Mcilroy. When he
and Dennis saw the power of pipes, they re-wrote all of their utilies
that processed something to reflect this new feature (mainly removing
console output). This is where the idea of a Unix filter comes from.
Ken's favorite thing to do with pipes was pipe dc (desktop calculator) to
a program that converted numbers to words, then pipe that to a speech
synthesizer.

Another important part to the story of Unix is a particular utility
called grep, which is very useful, even today. This was still before C,
so the original version of grep would have been in Assembly language.
Douglas Mcilroy asked Ken if he could write a program that would search
for things in files, and Ken used that night to clean up his already
made personal utility (it wasn't called grep then). The next day he
presented Douglas with grep and it has lived in /bin ever since.

There is one more piece of history to talk about before we get to the C
programming language, and that is the B programming language. Douglas
Mcilroy had written a TransMoGrifier (TMG) compiler in TMG (originally on
paper) that he got working on Ken's PDP-7. Ken wanted to offer Fortran on
every computer, so he began to work on an implementation in TMG. The
PDP-7 only had 4k machine words or about 9.2 KB of space available. Ken
used a second disk that contained identical B source code to work around
the limitation of space until B was small enough to run without the extra
disk. When Ken got B to what he considered a finished state, Douglas
wrote a compiler for B which was externally ported to several
universities. At this point the decision was made to make a higher level
programming language, the legendary C.

The early version of C and B were similar except for C had types, where
as B only a single type (machine word). After three failed attempts to
re-write the Unix kernel in the new C language, structs were added, and
Unix now worked on the PDP-11 written entirely in C. It has been 50 years
since then and C still remains as relevant today as it was back then.

Related:

* Brian Kernighan interviews Ken Thompson
	<https://web.archive.org/web/20190507080117/https://www.youtube.com/watch?v=EY6q5dv_B-o>
* The Evolution of the Unix Time-Sharing System
	<https://web.archive.org/web/19980220175817/http://cm.bell-labs.com/cm/cs/who/dmr/hist.html>

SKUTTER
=======

By Bodge N Hackitt

In these articles I will be describing some
experiments into controlling real world
applications using various aspects of the
Raspberry Pi computer.

I was inspired to start this project when a
member of the Raspberry Pi forum brought to
my attention a low cost robotic arm kit that
could be controlled via a computer's USB port.
The arm reminded me of something called a
"skutter" from one of my favourite TV shows,
Red Dwarf (pictured right) that was on when I
was still growing up. I thought that, as the
Raspberry Pi is so small, has such low power
requirements and is still so useful as a
computer that I could easily combine the robot
arm with a kind of motorised base and have
the whole thing run from batteries and
powered by a Raspberry Pi which would act
as the Skutter's 'brain'

It seemed to me that this would make a fun
kind of project which could even have some
serious applications. Imagine if you could
make an intelligent robot that was able to run
about on its wheels and manipulate things in
the real world with its robotic arm. Yes, it could
be fun just in its own sense but also it could be
of tremendous use for people with disabilities.
It might even one day be useful as a kind of
fix-it bot that could access small spaces where
people would find it difficult or dangerous to
get to.

In order to accomplish this, the Raspberry Pi
has two interfaces which will allow us access
to control stuff. The first of these is a kind of
standard interface which almost all modern
computers have built in. It's called a "USB" or
Universal Serial Bus.

I will explain how some elements of USB work
in the next article, but it is worth noting here
that this little port that we take for granted is
extremely complicated. Fortunately there are
some things which will make our work with this
easier.

The second of these interfaces on the
Raspberry Pi is called the GPIO which stands
for General Purpose Input (and) Output. This
part of the Raspberry Pi promises to allow the
user to easily control all manner of devices but
at the time of writing this article the Raspberry
Pi is not available.

This means that the first of these experiments
will be carried out using a "virtual" Raspberry
Pi running on a PC (This is not strictly true, a
proper virtual RasPi would involve
programming a simulation of the ARM
processor, its memory, storage and all its
other associated parts. My "virtual" Raspberry
Pi is actually just a minimal installation of
Debian-Linux (the operating system) that's
running on a program called Oracle Virtual
Box. Luckily this set up does give me access
to the USB port and this should work exactly
the same in this virtual implementation as it
would on the real thing. (Sadly, at the moment
we can't try things that would use the GPIO as
there is currently no straightforward way of
making a virtual Raspberry Pi with a virtual
GPIO header).

The robotic arm kit called the "OWI Edge" is
currently available from Maplin electronics and
it uses a simple USB interface to control it.

This kit is sold with a CD ROM with software
that will allow you to control it from a Windows
PC. The software allows you to remote control
the robot arm or to make a sequence of
instructions that controls it by setting the time
and direction that each joint should move. The
design of this robot and software is very
limited. The software only allows for the most
basic of programming and movement and the
arm itself has no feedback. This means that,
as it is we have no way of knowing what the
arm is doing other than by looking at it
ourselves.

A truly useful robot needs to know itself where
it is in space. In theory we should be able to
say to it "Get the object over there" and the
robot will know I am *"here"* and I need to be
*"there"* To get to *"there"* I must move by *"this"*
much and in *"that"* direction.

To make this simple robotic arm into a more
useful device we will need to do some
'hacking' and make some modifications.

As this project progresses we will cover some
ways of adding simple *"feedback"* to our
robotic arm so that it will know where each
arm part is in the space around it (its
environment).

We will also investigate some more advanced
methods of giving our robot a kind of sense of
sight by using "sonar" and we will consider
some further possible applications of machine
vision using cameras.

When the actual Raspberry Pi computer
becomes available we will be able to start to
put things together properly and begin to
construct our motorised base

In the next article I will cover methods of
controlling the robotic arm via the USB by
writing instructions in the Python
programming language. Looking forward to
seeing some of you again then.

Article by Bodge N Hackitt

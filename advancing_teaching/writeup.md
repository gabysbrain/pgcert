---
title: Improving my teaching and assessment processes
author: Thomas Torsney-Weir (849707)
bibliography: writeup.bib
---


# Intro


I want to improve both my delivery in teaching as well as assessment of the
students. I want to improve the timing of my lectures and implement automated
grading of assignments. In many ways, both these improvements are about being
efficient with my time. This efficiency will hopefully mean more time for
effective feedback and discussions.  For both of these areas, I will be using
the experiential learning cycle according to Kolb[@kolb:1984]. This is a
four-stage model which starts with identifying an experience, reflecting on it,
developing a plan of improvement, and finally implementing that plan. 


# Teaching

Now that I've been doing lectures for a number of years, it has become
relatively easy to fill time. I can put together a basic set of materials to
fill the time. My initial worries about not having enough material to fill the
time turned out to be short-lived. I can now fill as much time as need be and
explain what I mean to every lecture. However, this has caused a new problem.
Now, my lectures often run long. I try to cover one topic per lecture or split
long topics into two lectures. However, due to student questions and off-hand
discussions my lectures can often run long and I end up dedicating 90 minutes
total to a topic where I only meant to spend 50 minutes. Questions are
unanticipated.  Every semester brings a new set of questions and discussions. I
also try and incorporate major questions from previous semesters into following
ones.  This means that I may need to either shorten a lecture later in the
semester or remove a topic entirely. I need to work more on managing time
during my lectures.

The prevailing advice on timing during lectures mostly comes from general
presentation advice. For example, planning on taking one or two minutes per
slide, ensuring that slides are clean and clear[@reynolds:2012], mark timing
information in the slides, and extensive rehearsal[@bligh:2000]. The underlying
assumption is that, with enough preparation, one can keep things easily within
the time allotment. I have followed this advice myself, even before lecturing,
for my own conference presentations to great success. 

I find that this advice works well for conference talks but does not always
transition well to a lecture environment. A conference talk is a very
controlled environment. You are allocated a certain amount of time for a
presentation and then there is a dedicated time for questions. This is very
different from a lecture environment, at least the way I think lectures should
be. Students are encouraged to interrupt and ask questions at any time. These
questions might lead to a longer discussion which can take up enough of the
lecture time that I will not be able to finish my prepared material. The
students really appreciate this time, it is more interesting for me, and it 
is a good gauge for the degree to which students are paying attention. I think
students should always be able to interrupt when questions or discussion points
arise.

There are a few solutions to this from my perspective. One is to tell students
to hold all questions until the end of the lecture. Basically, this would make
all lectures into the conference talk framework. This is actually easier now
with online lectures. Students engage in my lectures through the text chat
feature rather than voicing questions. Students can write their questions when
they come up and send them and I can go through them after the lecture.  With
face to face lectures, students would have to write their questions down
somewhere. I really don't like this approach. Students may want be asking a
question for clarification. Without this, they may be lost for the rest of the
lecture. Once their question is answered, the rest of the lecture will not
'magically' make sense suddenly. They will have to go back and watch the
lecture again. That sounds quite discouraging to me! Furthermore, students may
forget the reason for their question in the first place. There have definitely
been conference talks where I have written down a question only to have
forgotten the reason for it by the end of the talk. Surely, in a learning
situation, this will also be the case. Finally, I never liked the lectures 
where questions had to be held until the end. It was quite frustrating and it
discouraged engagement with the lecturer.

So, my plan going forward is to restructure the order of delivery of my
lectures. Right now they are in a 'standard talk format' where each slide
builds on the last. The material students need for the exam is intermixed with
additional guidelines and examples. It is difficult to skip slides given this
format. I think it will work better if I restructure my lecture to have 25 to 30
minutes of the material needed for the exam and then leave the 'nice to knows'
for the last part of the lecture. I can skip these items at will if required 
or go over them if there is more time available. That will require some work
tying the narrative together in a logical way, but with practice that should
become easier. Then, I will not need to worry as much about how long my 
lectures will take.

# Assessment

One of the persistent issues I have with assessment is with maintaining
consistency of marks across a set of students. As I go through a coursework it
is difficult to remember all special cases where I deducted points.
Furthermore, marking Computer Science coursework requires a lot of detailed
inspection of code and small mistakes may have major implications. Repeated
detailed tasks mean that many mistakes will be made.  This is annoying but
manageable in modules with 30 students but extremely time consuming in modules
with 130 students. 

The prevailing advice to deal with this is to develop a marking scheme before
going through the assignments. I would then refine this scheme after marking a
few randomly selected assignments. The idea is that then I can refer to this
while marking. This method is very helpful for keeping things consistent across
students.  However, this doesn't address the issue of finding detailed coding
errors in a large number of submissions. Automated marking, just like automated
testing in production environments[@beck:2003], will find these detail errors
faster and better than I can by hand.

I have tried using automatic tests in assignments to cover this in the past.
There are a number of positive stories about how this has made marking
consistent and efficient[@blumenstein:2004;@striewe:2009;@edwards:2007]. However,
I find that many students are unfamiliar with automated testing and have
trouble implementing code that can be run by the tests. It seems unfair for a
student to completely fail an assignment because they missed some minor element
of the assignment. Computers, and code tests in particular, are not very
flexible. In addition, the automation makes it easy for me to miss certain
special cases.


In the real-world, software is developed and tested extensively using automated
methods[@beck:2003]. Therefore, these automated marking systems will give
students practical software development experience.  It is not a trivial matter
to implement automated grading. The practical issues are balancing the issues
of avoiding grade optimisation and code that cannot be easily tested. I also
want to encourage creativity and flexibility in terms of how they design
software.  As an example, I am teaching a database module and the students are
free to design the database as they see fit. It is not possible to write a
testing script that will load data into an unknown data structure.  One option
is to allow students to edit the tests themselves, although I worry that this
will just lead to increased grade optimisation.

While this has been implemented by a number of my colleagues to varying
degrees, addressing all these issues will require a number of iterations to get
an effective system working.  I think automated marking can help but mostly as
a guide for pointing to where are issues in the code.  I want to tell students
beforehand that this will be to identify key issues rather than being the
single point of marking.  This means that students won't have to adhere
perfectly to the marking schema. Mistakes will still show up as errors in the
testing system but upon further, manual inspection I can address these.
Students can have access to the marking test suite so that they can make sure
things do not break on submission. 


# Conclusion

Improving both the efficiency of my time delivering lectures as well as marking
coursework will increase the amount of time I have available for other aspects
of my job. I can devote this time to additional research or restructuring
modules.


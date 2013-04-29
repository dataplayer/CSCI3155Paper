I wasn't comfortable with the html file that Nic sent out, so I started work in in MD. I left numbers in just to indicate what I was thinking of including on each slide. Clearly we'll need to move things around and modify them - and delete the numbers.

1
Classes: The New Sugar in JavaScript
====================================

By Nicandro Flores, Megan Greening, and Brian McWilliams
--------------------------------------------------------

2
How did we get here?
====================

*ECMAScript is a specification for scripting languages
*TC39 is tasked with writing the new spec, called Harmony or ECMAScript 6 (ES6)
*Classes will be added in Harmony
* Programmers are divided on whether or not this is a good thing

3
The Prototypal Way
==================

*JS is object oriented, but it doesn't have Class syntax, as Java does
*Classes can be simulated in JS since objects are highly versatile
*"Prototype" is the property that allows programmers to simluate protoype-based classes

4
Code Example of Prototypes
==========================
*Some or all of the employee example? This might be two slides' worth.

5
More Code to Complete Protype Discussion
========================================

6
Maximally Minimal Classes - What Do Classes Need?
=================================================
*A Class keyword 
*A body that includes the constructor function and instance methods
*Cand declare a class as a subclass of another class using extends
*Super is available from any of the methods or the constructor

7
Formal Class Grammar
====================
<Note/speaking> When we began gathering resources for this topic, we were suprised to be able to apply what we just learned.  The task group was describing the new feature in Backus–Naur Form.   Here we see the top level Class definition.  It is a little harder to make out than what we did, but we can see that ClassDeclaration returns a Binding Identifier and a Class Tail, then a ClassTail.
<End speaking><p>
<center>Class BNF</center>
<pre>
ClassDeclaration: class BindingIdentifier ClassTail
ClassExpression: class BindingIdentifieropt ClassTail
ClassTail: ClassHeritageopt{ ClassBodyopt}
ClassHeritage : extends AssignmentExpression 
ClassBody: ClassElementList 
ClassElementList: 
    ClassElement 
    ClassElementList ClassElement 
ClassElement:
    MethodDefinition;
MethodDefinition :
    PropertyName(FormalParameterList) {FunctionBody}
    *PropertyName(FormalParameterList){FunctionBody}
    get PropertyName ( ){FunctionBody}
    set PropertyName(PropertySetParameterList) {FunctionBody}
</pre>
<align = right>
July 26, 2012 TC39 Meeting Notes Allen Wirfs-Brock http://t.co/PwuF12Y0
</align>

From Prototype to Class
=======================
*Put code here that relates to previous code, discuss differences

9
How Classes Will Be Used
========================
*Put code that shows how classes work.

10
Pros
====
*I'll leave several sections blank - we can move stuff around as we need to.

11

12

13

14

15
Arguments Against
=================
*Why add something to JS that we can already do?
*Remember, protypal classes are available and they work!

16
Additional Confusion
====================
*Adding classes creates two main areas of confusion
*Adding common features of classes (inheritance, subclasses, etc) add confusion
*There will be TWO ways of creating classes and that may lead to errors later on

17
Why The Prototypal Way Is Good
==============================
*Code snippet that show it is essentially the same as classes

18
What's the Point of Minimal Classes?
====================================
*Minimal classes are limited.
*Classes may be introduced in late 2013, but it will take a lot of time before they are in regular use.

19
Conclusion
==========
*The decision has been made and classes are coming to JS.
*The good news is that under the hood classes just use the structure that JS already has to work: that means that, in theory, everybody can be happy!

20
Closing Thoughts/Extra Slide/More Conclusions
=============================================

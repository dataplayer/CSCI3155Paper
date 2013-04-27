The New Sugar In Your JavaScript
=================================
Group Members: Nicandro Flores, Megan Greening, and Brian McWilliams.

ECMAScript is an internationally standardized specification for scripting languages.  Many client side languages such as JavaScript(JS) and ActionScript are derived from it.  TC39 is a working group tasked with the responsibility of writing the new ECEMAScript 6 (ES6) specification[1], with a late 2013 target release. In approximately six months Node.js will begin embracing the newly proposed specification, browsers will begin popping up messages asking users upgrade their browsers, and JavaScript (JS) programmers will stand divided with TC39's decision to include a new class syntax into the language. 
The Prototypla Way
------------------

Despite JS being an object oriented language it does not have syntax to create classes in the conventional way programmers are used to, such as in Java. ECMAScript does specify that program state and methods are carried by objects, and that structure and behavior are both inherited. Therefore, even though class syntax such as "class" and "extends" do not exist in JS, there must be a way to simulate the idea of classes in JS. 

JS function objects are highly versatile. They are first class citizens, thus are treated like data just as classes are in other class based languages. For example, functions in JS can be used as templates to construct other objects. The templated objects are easily created using the 'new' operator. In addition, they come pre-equipped with hidden properties and methods. One of these properties is the 'prototype' property, with these three tools programmers can simulate prototyped-based classes. 

==== Insert example of a prototype based class here ====
>> Use example mentioned in the link below
>> here: http://www.2ality.com/2011/11/javascript-classes.html
>> If we need other examples use:
>> http://www.2ality.com/2012/01/js-inheritance-by-example.html
>> Point out the use of call(), may need to meniton apply() and bind() too
>> and how they are used to switch context.
>> Point out the renaming of Employee.prototype.constructor to Employee which
>> examplained here:
>> http://www.2ality.com/2011/06/constructor-property.html

>> lead into next topic saying like:
>> "Does JS need a native syntax to shorten the above example?"

The new Class Syntax
--------------------

>> Classes added to ECMAScript.next on 2012-07-29
>> Mention the new class syntax: "class","constructor","extends","super"
>> If we can describe how these work.
>> They are just sugar for what we describe above.
>> Many JS libraries use this. Prototype.js, CoffeScript, etc.
>> The new class language is mentioned defined here:
>> http://people.mozilla.org/~jorendorff/es6-draft.html#sec-13.5


Arguments for
--------------

>> make it easy for new JS programmers
>> similar to what other seasoned programmers are used to
>> Lost of discussion here:
>> https://mail.mozilla.org/pipermail/es-discuss/2012-May/thread.html#22825
Progammers working in other languages are used to be able to work with classes in their code. By adding this functionality, JS would be brought closer into line with other languages. It seems like there is popular support in the JS community for adding classes. However, as with any new modification, there is some concern over how classes will be implemented.


Arguments against
-----------------

>> lost of arguments here:
http://www.nczonline.net/blog/2012/10/16/does-javascript-need-classes/
>> This will clearly needed to be edited for clarity, but I really wanted to get some ideas in writing. -MG

While it seems like the general consensus in the field is that adding classes to JS will be a good thing, there are those who do not see a need for classes. Many people argue that you do not need classes in JS because there are already ways to effectively create "classes" through the use of constructors to define custom reference types. Furthermore, they feel that common features of classes (subclasses, superclasses, inheritance, etc) tend to cause additional confusion. You can already create custom reference types and all this change will do is to add unecessary syntactic sugar. Since the addition of classes does not alter how JS works, why bother adding it?

The addition of classes is merely a simplified way of using the features already avaialbe to JS. Many feel that you should just learn how to use the syntax already available to you. No major change is occuring - in essence, all that is happening is the the underworkings of the code are being hidden by the new class syntax. Prototypal inheritance is not that confusing once you start getting down to the details of it - and it even allows for inheritance.

Concluson
--------- 

The new class syntax proposed by in the new ECMAScript.next hides the standard details of writing prototypical classes in JS. Is hiding the details a good thing? New programmers may not understand what is going on under the hood when things go wrong when using the new syntax. The new syntax will certainly lead to nicer symantics and new JS code produced with it will be more readable and clear. At what point do we decide we've had enough turtles, Feyman? Future generations can decide this. 


Slides for talk
================
5 mins worth:
>> use code snippet above to explain prototypical classes
>> use code snippet above to explain new syntax
>> mention how the new syntax is just sugar for what we are used to doing
>> mention how the new syntax works
>> don't allow time for questions! haha

Citations
---------
[1] Draft Specification for ES.next (Ecma-262 Edition 6) [Online] Available: http://wiki.ecmascript.org/doku.php?id=harmony:specification_drafts

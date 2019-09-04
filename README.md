# Sculpting Software

## An interactive essay on Behavioral Programming

Automation has taken over many things in our society: agriculture, medicine, transport, entertainment. Many say that the future depends on software; unprecedented global problems are already in a state of no-return and fixing these problems will require unseen complex technological systems, most likely driven by software. The way we control these layers of automation, that we have become so dependent on, is through "programming".

The problem seems that we (humans) have to abnormally force our minds to learn programming. We adapt our unskilled reasoning to work in the way the computer wants. As the layers of abstractions and patterns grow bigger and stronger, the same fundamental issue remains: programming is an unnatural process that will forever require us to override our natural model of thinking in order to learn to think like a computer. 

What if we could take the opposite road: **figure out which paradigms best fits our model of thinking**; since that is precisely one thing that will hardly change.

In this article we will take a look at how ``non-coders''  understand and make changes to complex systems. We believe that analyzing how we naturally describe things, without having to think like a computer, will give us great insight into key properties that may drive future programming paradigms.

### Introduction

Programming is hard. It is mostly a process of "overriding our natural senses". After all, this is what we do in most cases when learning other fields: the natural world does not own us a universe we can easily understand.

But can we think of programming without a computer? We believe important insights can be found when observing how "non-coders" think about systems. Specifically we notice a common pattern for developing software: requirements are created in a form that is understood by most stakeholders. These requirements can take various structures: a simple list of instructions written in textual form; diagrams and flows of information drawn as boxes and arrows; and much more.

Since this is what non-coders do, it seems reasonable to think that it is the highest, purest and most natural form of programming. Doing anything else -- we want to emphasize on the *anything* -- would be falling into the trap of what the computers want us to do.

After analyzing important properties emergent from how we construct and maintain requirements, we will apply these properties to actual programming paradigms. Hoping to answer the question: can the requirements become the final implementation?

### Programming a system by discussing with it

Usually we maintain and develop a system by creating an artifact which contains all the instructions we want the computer to execute. This artifact is composed of small pieces, modules, functions; hence we can reason about pieces independently. Sometimes we also execute pieces independently to see whether they work properly (unit tests). However the issue of understanding and changing the system still remains: we have to read through code, understand where to squeeze new code to implement specific requirements. 

We think there can be another way of developing systems that is similar to how we discuss with other humans. In this analogy we do not need to read or maintain a single artifact; rather, we can discuss with it to both (i) understand how and if it can do something and (ii) change how it does something. For instance let's take a look at this conversation between human (H) and computer (C):

```
H: “When the driver presses the brake pedal the brake light should turn on.”
C: “Does this apply also to when the engine is off?”
H: “No.”
C: “Done.”
```

And later:

```
H: “I saw the car rolling downhill and stopping; how did it stop?”
C: “The driver pressed the brake pedal.”
H: “Why didn’t the brake light go on?”
C: “The engine was off.”
H: “The light should have turned on anyway.”
C: “But earlier you said no.”
H: “Ah, right. So please remove this exception.”
```

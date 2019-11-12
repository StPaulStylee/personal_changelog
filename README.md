# personal_changelog

### 11/4/19
I was unable to begin my Game Development Systems programming because I cannot remote into my CPU (I'm traveling for work). However, I continued my Design Patterns study. Tonight I began studying the Strategy Pattern. Basically, you create families of behaviors (interface) that are then implemented by a class. That class should then be used to by a parent/subclass. The whole idea is to allow for flexibility (composition nover inheritance).

### 11/6/19
I began my study on the observer pattern - only introductory study, no implementation details. Basically, you have publishers (Subject Object) and subscribers (observers). The observers subscribe to the subject object (or a bit of data that the subject object owns) and when that data changes, the observers are notified. If the observers no longer wish to receive updates, they can unsubscribe from the subject object.  It's similar to a newspaper subscription model.

### 11/7/19
I was unable to complete my commitment for today. I came home from a business trip late last night so I slept as late as possible this AM. The kids just went to bed and I am beat. I am logging here tonight as a reminder that I will be continuing to build this habit, even if I miss a day here or there. I'm up at 5 AM tomorrow, ready to start my game systems programming!

### 11/8/19
I typically sleep with ear plugs since my wife tends to snore 😬. Usually I can set my alarm and still be woken by it regardless of the plugs... Not this AM though. So, I had to further delay my system learning.
However, I did continue my reading on design patterns and the Observer pattern in particular. In a standard implementation, you great two interface types... A Subject interface that defines a register, unregister, and notify method. Second, you create an Observer interface that has an update definition. I'll get into further details tomorrow.
Further, I watched a short tutorial on You tube about using the Observer pattern in Unity3d. The video contained two implementation patterns... One was basically what I just described... But the second was setup using built in C# events - Action. 

### 11/11/19
Well, the weekend was rough. We drove halfway acroos North America, so I'll try and cut myself some slack. Tonight I was able to begin my study of VG Systems programming in Unity. The first thing I am tackling is Character and NPC Navigation systems. I wasn't able to get too in depth tonight as I was setting up the project and all that boring starter stuff. I was able to learn about a cool bit of C# though, which is the 'out' keyword. Basically, the 'out' keyword allows you to pass a method argument by reference (like a pointer?) and not by value. What's cool about it is that the argument does not have to be defined prior to passing it as an argument. This differs from the 'ref' keyword in that the 'ref' variable must be defined prior to its use. This also differs in from the 'in' keyword in that with 'in' the argument must be defined and it cannot be edited within the method which it was passed (read-only).

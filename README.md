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

### 11/12/19
Today I did some more learning on design patterns - I couldn't find time tonight to do game dev stuff. So, the pattern I learned about tonight was the Adapter pattern. The pattern aims to take two incompatible interfaces and allow them to work together - typically, this is necessary when one/both/all interfaces cannot be refactored. In other words, getting a new class designstructure to work with some legacy classes. To do this, you use a sort of "man in the middle" approach - the adapter. Overall there are 3/4 players in this pattern. The client - the new class/source or whatever - that isn't compatible with the leagacy stuff (the adaptee). The target - an interface or class (this is where the +/-1 comes from) that implements the methods that the client will use. Usually the target inherits the client class and then implements the interface (if necessary) and the adapter also has reference to the adaptee, so it can make the necessary reconilliations between the client and the adaptee. And lastly, the adaptee, which is the legacy shit. Pretty cool, and useful at work as we are constantly looking for areas of modernization and this is a good bridge in doing that.

### 11/13/19
A couple of days ago I began a Navigation system tutorial. I could tell almost immediately that the resource was a poor fit for me, so I have pivoted to some resources via Zenva Academy. I've used them before and been very pleased. I've been forced to pivot a bit though in that they don't have specific "systems" courses, however they have a "RPG" path which will cover many different systems throughout the content. So, I got started today... didn't get any programming in but I built a tile map for a "mini" 2D RPG. So, I learned how to create a tilemap and then create a tile pallete to paint on the tilemap.

### 11/14/19
Today I set up the basic player movement in the mini rpg project I am working on. Not only does the player move, but the sprite changes directions depending on the direction that the player is moving. This project is using the older input system to do the controls... And that is ok. I have experiemented with the new input system that is in still in preview and while it seems nice and easy for settin up multiple input systems... implementing them seems much more verbose than the current system. I could be wrong in that I have introdcutory knowledge of both, but this is my first impression. Hopefully soon I can get beyond some of this stuff that is more introductory - although it is good reinforcment of the fundamentals - and more into the systems programming that was the aim of this challenge. Regardless, I am having fun and learning, which is NICE!

### 11/15/19
Today I set up the enemy movement system and the player attack system. While both very simple implementations, I did learn some cool stuff about game development in Unity. In order to get the enemy to move appropriately - in more of a chasing implementation - I needed to calculate the distance from the enemy and the player, and then normalize that value so it is easier to apply a predictable speed value to the enemies movement. It was a good learning experience cause I had no idea what normalize was... In simple terms, it takes the magnitude of the direction the enemy will need to move to move towards the player (magnitude is the sqr rt of x * x + y * y + z * z) and reduces the magnitutde toa value of 1 or -1. This is useful because you then can predictable calculate the velocity of the enemy when you want to move it. The player attack system was useful as well in that I solidified my understanding of what a Raycast is - basically just a one directional line that when it hits a collider, sends data back on collision. I also used some overload parameters such as a layer mask to only calculate collsions with an enemy. Good stuff today!

### 11/16/19
Pretty light day today... I implemented the Enemy attack system. It was fairly straightfoward... So not much "change" to report in the changelog, but alas, not everyday can be a winner! One thing I am noticing is that there is a lot of room for improvement within the code. So, at the end I'll either refactor the code correctly, or I'll make my own little project that basically replicates this one, as an excercise in retention, and I'll write the code better in that project. 

### 11/19/19
I've missed the last 2 days while we were driving across the country, so that's unfortunate. This AM I continued to work in this "mini" RPG - I implemented a small particle effect when the player successfully attacks an enemy. This is my first experience using the particle system. It was a pretty quick overview and we didn't get too much into details, but it was a good first exposure to something that is extremely important in game development. I am excited to use this experience to begin creating cool particle effects in the future. With that said, this is not really the systems programming that I had committed too, but that is ok... Tomorrow I will begin implementing a leveling system using XP gained from combat... I am sure it will be a very simple implementation, but growth comes in small, incremental steps!

### 11/20/19
TOnight I implemented a very simply leveling system for the player. Super duper basic, but a simple implementation is nice as a foundational exercise.

### 11/21/19
I took a break tonight to revisit my design patterns book. I am still reading over the Observer pattern. I actually had to go back and refresh myself a bit... So I only really read a couple new pages. I was asked to complete an exercise in implementation of the pattern before the book showed us an implemented. From what I can tell, I did aight. 

### 11/22/19
I finished the chapter on the Observer pattern tonight. We went into implementation details and they are super straight forward. Not really even worth rehashing asnive already described it above. Good though, and I am anxious to get an opportunity to implement the pattern at work. 


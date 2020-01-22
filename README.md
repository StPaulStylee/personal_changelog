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

### 11/24/19
I finished the chapter on the Observer pattern tonight. We went into implementation details and they are super straight forward. Not really even worth rehashing asnive already described it above. Good though, and I am anxious to get an opportunity to implement the pattern at work. 

### 11/25/2019
This morning I was able to complete the UI System for the mini-rpg. This was my first exposure to the TextMeshPro package within Unity - it was very simply however. I'd say that today I didn't learn a whole lot that I didn't already know, but I am beginning to feel very comfortable inside of the Unity editor - understanding when a new layer is necessary, how to navigate different preferences, etc. Up next is a event driven inventory system. I am excited to see how we implement it and I hope to get some new perspectives out of it.

### 11/26/2019
Today I began implementing the interaction system - loot collection, basically. This is done using the UnityEvent object and the Unity editor. In the passed, Inhad implemented some events using the C# delegate keyword... But this was much more straight forward. I'm going to look back at those passed implementations and see how they differ from this Unity based one because I am curious if one is more optimal than the other in different situations.
Also today, I was listening to a podcast about Game Design - I want to get into game programming but I still live listening to these things - and one episode emphasized the need for a portfolio. I am going to start building one. I'm not sure what my strategy is quite yet, but I am going to put a plan together and start working. My gonasbof now - and this is open to extension - is to have a portfolio large enough to confidently apply for work in the game programming space by the end of 2020.

### 11/27/19
This AM I continued implementing the interaction system. Now the player can loot crates and also enter buildings - the way this is done is I created another tile map off camera and I simply transport the player and the camera over there... It's pretty neat. So, how did I grow today? Well, I suppose I got a better grasp on how to set up the camera to follow the player. There is room for improvement here... The camera currently follows the player but has no knowledge of the edge of the tile map. This can cause the camera to render outside the edges of the tile map, which looks pretty bad. I imagine we would need some sort of logic and/or in editor components to stop the camera movement along a particular axis if the player character is appoaching the edge of the tile map.

### 11/28/2019
Thanksgiving, what a great holiday, but a tough one for productivity. I wasn't able to do any coding today as I spent all of my free time researching my next CPU build, which I will be buying tomorrow!!! So I suppose I did grow a bit... I refreshed myself on CPU hardware and I also grew on excitement about a new computer!!!

### 01/02/2020
It's the start of the new year and I have a number of personal goals for it. One is to read at least 2 technical book - one every 2 quarters. Also, I am dedicating my free time coding to video game development. I want to decide if this is really something I want to pursue further, perhaps, as a career. So, tonight I picked up my design patterns book and began reading it again. Today, we started reading about the decorator pattern and it's adherence to the Open/closed principle. What is that? It means writing code that is open for extension but closed for modification? In other words, you want to write your code in such a way that if a feature needs new functionality, the cooder can easily implement that by extending the code and leaving all existing code untouched. It's important to use this principle with good judgement as overuse will leave your code unnecessarily complex. Try and pinpoint the areas of the code that are most likely to change, and implement it there. I haven't got into any implementation details yet.

### 01/03/2020
This morning I did a little game development... I am continuing to work on a very basic RPG - basically a rehash of a tutorial I complete, but this time I am doing it on my own. I am nearly finished. I implemented some of the UI today - the players health bar, xp bar, and current level all update and render as expected. This type of work is becoming easier in that I no longer need notes/tutorial to help me implement. This is great because now I have enough proficiency to start focusing on more advanced UIs.

### 01/04/2020
This afternoon I nearly completed my rehash of the basic RPG game. I implemented the interaction system - Item pick, building entry, Xp pickup, etc. I also implemented a basic camera follow. Tomorrow I want to refactor all of the code so that it uses proper design patterns and class structure... Right now, it's pretty hideous. I am finding that I know how to complete some tasks without having to reference any materials. So I am growing in comfortability which is great because it means I am getting ready to start taking on more complex games. YEAH YEAH YEAH!

### 01/06/2020
This morning I completed my rehash of a very basic RPG. I completed implementing the inventory system and then refactored by character classes to inherit from a base abstract character class that contains a few different abstract and virtual methods. This has been a great experience. I am feeling ready to take on something new and challenging - this is the most comfortable I have felt with Unity and C# in general. That is not to say I still don't have A LOT TO LEARN, but I feel that I am in a place to start learning advanced topics and do so effectively.

### 01/10/2020
I've missed the passed few days : ( With two young kids, sometimes it's hard to find the time I need. ANyways, this morning I started a new project where I will be implementing some interactable NPCs, a gateway system, a camera that stays within the bounds of the map, and a dialogue system. Specifically this AM, I learned how to use something called a "Rule Tile". The rule tile is a sprite that is used to create a tile map and the sprite has specific rules set to it. Depending on what the logic tells it, particular sprites will be rendered. It's pretty neat and useful for designing a 2D map. It will be good to have experience with this as a well rounded independent game developer despite this not being my real passion which is the programming side of game dev. Regardless, I am having fun and learning mroe about develepment within Unity.

### 01/13/2020
We used some Unity Editor tools that are not standard but available via Github. The Rule Tile and Prefab Brush. The Rule Tile allows you to set rules on a certain tile in your tile set and depending on the rules, paint a particular tile. This would take some practice to really become proficient with but it is a good tool to have awareness of just in case you need to use it or make reference to it’s existance in a job interview or as a viable tool for a project.
The prefab brush is something I can see as a little more useful. To use it, you first must make create a prefab brush in Assets < Create < Brush < Prefab Brush From there you give it name and a size (the size sets how many objects will be assigned to the brush). You then need to create a new prefab and assign it a collider (this is the use case for this project). You can then assign the prefab to the brush and use the brush in your tile pallet. The use case in this project is to make a prefab brush that we can use to paint box colliders on interactable objects such as doors. 
Another cool thing we have done in this project is make use of multiple layers in our tile/grid. This allows me to set different types of tile layers for our tile map and set each layer to a particle layer value - eliminating the need to rely on the Z positin value available in the tile pallete. 

### 01/14/2020
Not a lot of new learning today. I created another scene for this RPG Town tutorial I am doing and continued to solidify some of the stuff from earlier lessons. I have just begun to create the character class that both the player and NPCs will inherit from, but nothing ground breaking yet. 

### 01/15/2020
My son woke up super early this AM so I didn't get as much time as I had wanted. One new thing I learned about today is that in your class declarations in Unity, you can require that class to have certain components. Using an attribute on the class declaration itself, you can create a list of components that are required for the class. When you assign these classes to a game object within the Unity editor, they will automatically have those required components assigned to them. Further, you cannot remove the required components within the editor... Pretty neat.

### 01/16/2020
Today I finished implementing the NPC movement system. Very basic in that the NPC only moves 1 tile in any direction, and then back to there starting point. This is good exposure to how these movement systems can be implemented, even if it is very basic. I am continuing to learn the foundations of game development and that is very exciting. As I continue to say, I am setting myself up to learn more advanced techniques. I love this ish. Oh, and I also learned the difference between IEnumerable and IEnumerator in C#. The StartCoroutine method in Unity requires a method that returns an IEnumerator... I am guessing this has something to do with the fact that the StartCoroutine method needs to be able to track the state of Couroutine method that is passed as an argument to StartCoroutine... I am not certain of this, but it's cool to know the difference either way. 

### 01/17/2020
We created a Gateway class and a Gateway Manager. The manager is a Singleton. Each possible gateway (a door for example) has a gateway script on it. The script has a property for the scene to be loaded as well as the position that the player should be put into the new scene. The gateway then calls the singleton manager in which the manager performs the necessary logic to set the spawn location and move the player to the spawn point, then the gateway class loads the scene. It is important to remember that each scene must contain your player prefab in it in order for this implementation to work. 

Cinemachine! Baller. This thing is going to take a whole tutorial on its own to really get a feel for it but man... This tool seems amazing. I'm very excited to jump into Cinemachine in the near future as camera work is essential for quality games.

### 01/22/2020
I actually put time in yesterday too, but forgot to update this log. Whoops! So, scriptable objects... These are used to add data to a game object in a modular manner. To create one, you simply inherit yuor class from ScriptableObject. You can then add a attribute to your class called “CreateAssetMenu” which allows you to place this scriptable object in the asset menu and create it on demand. With this attribute you can assign in a filename (not sure how we use this yet but I am sure I will find out) and the name of the asset in the asset menu. In this course we used the ScriptableObject to create a dialogue object that we could assign to our NPCs.


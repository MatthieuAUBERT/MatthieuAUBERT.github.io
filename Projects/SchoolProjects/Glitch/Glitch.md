# Glitch

> How to Fix 404 - Student's Studio for the 5th Semester of ESMA's Game Design formation, composed of 6 members.
> 
> As a Tech Artist / VFX Artist
> 
> September 2022 to June 2023
> 
> Unreal Engine 4.27

![BG](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/SchoolProjects/Glitch/Images/BG_Glitch_2.png)

## Quick Pitch

Glitch is a Tower Defense and Stealth game on PC where the player embodies a character to the 3rd person view. That character evolves within a medieval world corrupted by a strange void.
Fighting this corruption generates singularities in the whole world.

Players will have to progress quietly inside the void world to identify key structures and capture them to bring back the world as it was. When the player finds his exploration is enough, he shall survive from multiple enemies incomming by creating his own defenses.

## My Works

At first, I made a lot of researches with my art director and our 3D artist to understand how can we bring this universe to life.The whole universe is between a medieval and a virtual world. That opens some opportunities of development but closes others.
It was pretty hard to start working from no visual. Collecting concept arts, suggesting ideas or even doing some tests like on how a particle reacts with a given node took some time but it was really helpful since I gained the time lost for the development part.

I also started using PopCornFX, a FX-Software, which have a great implementation pipeline with Unreal. Of course I had to learn few things with this soft (I'm thankful to the PopCorn's Staff that helped me) but for the development phase, I was totally ready.

What's important in making FX for this kind of game is to know the limit beyond Satisfaction and Comprehension. The dev phase was greatly around that. When I started developping an idea, I must keep in mind : Is it comprehensive ? What informations does it brings to the player ? And surely, is it optimal ?

Understanding all of that AND corresponding to the art direction was the challenge. I worked on creating particles effects that corresponds to the Towers, the Traps, the Environment of the world, the player's action and his avatar, enemies responses...

What was "simple" was having the validation of my art director. We have a heavily stylized game that I understand pretty fast. 

Here's some effects I developed (subject to change during next months) :

***Creating a Transition Between Two Connected Worlds***
> Using a Unreal Material I had to create an effect that brings a new visual to the world and can be reverted.

![TransitionShaderGIF](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/SchoolProjects/Glitch/Images/TransitionBetweenWorlds.gif)

![TransitionShader](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/SchoolProjects/Glitch/Images/NodalUnreal.png)

***Effects made with PopCornFX***

![Arrow](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/SchoolProjects/Glitch/Images/ArrowTrajectory.gif)

An effect that seems simple but was the most difficult one so far. I had to create the whole trajectory first by remembering math vectors. Then the mesh needed to be well oriented so I used a linear interpolation put with many vectors calculations to create an updating orientation. But the real difficulty was the implementation were I needed PopCornFX Staff. They learned me good practices when working with Physics node, Local/Global between Unreal and PopCornFX and so on.

![ElectricArcs](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/SchoolProjects/Glitch/Images/TowerElectricShot.gif)

An electrical tower shot that take two positions (the tower and a value returned by a raycast launched in a BP) in parameters and link them with electrical arcs made using "Beam Setup" Node. I added some others parameters like the intensity or the lifetime to improve the feeling and/or change the effect in engine.

![EnemyDeath](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/SchoolProjects/Glitch/Images/EnemyDeath.gif)

That one has a particular story. It was one of my first effect because I was trying to replicate a [Fire Plexus Tutorial](https://www.youtube.com/watch?v=vYom8JftGr0) to start using PopCornFX. And because I was using a far more recent version, it was impossible to perfectly replicate it like the video. But by learning spatial layers, I finally succeed. And this fire plexus, by changing some parameters, became an effect when the enemies will die.

![GlitchDash](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/SchoolProjects/Glitch/Images/GlitchDash.gif)

A quite simple effect that links two positions, a start and an end, and sends some particles. Some of them have a trail to make this rectangular effect. There's also a beam flash at the beginning and at the end followed by floating particles, giving a feeling of strength.

![Nexus](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/SchoolProjects/Glitch/Images/ChainedNexus.gif)

Here I add to make an effect that tells that an certain object is imprisoned by a virtual entity. This effect uses a simple texture put with many duplicates in a circle. And then I added an orbital movement to make the whole thing rotate around an axis.


## What I Learned

This project sure gave me the full comprehension of creating an effect from scratch. I learned some skills that will be usefull in the future such as tools versatility, thinking about others jobs by implementing variables to quickly change an effect and knowledges about Vector Fields (used a little) and PopCornFX's soft (used at 90% for effects) . That also gaves me the tools to understand how hard video game productions can be I'm happy that I worked in a healthy and efficient group, with people I didn't knew that much.

# My Portfolio

> The effects contained here are from my personal works. Under every effect, you can read a little explanation on how it was realized. There's also other effects that are waiting to be seen in the game "Glitch" I've produced for my last year project. You can find it in the [School Project](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/SchoolProjects/Projects.md) Page.

## My Works (Presented in a chronological order)

### Basis (or first effects that needed inspirations / researches)

![IceAttack](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/VFX/Basis/IceSpell.gif)

02/08/2022 : This effect has been created from references. It is composed of three VFX and two Shaders. The use of Blender has created relatively basic ice peaks. After modeling these peaks, it was enough to create the shaders and give a timing to all the "events" for the effect to have the desired impact. Thanks to the workflow used for this effect, it is extremely simple to make it more unpredictable, to change 3D models or even textures.

![Orb](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/VFX/Basis/Orb.gif)

27/07/2022 : For this effect, I used as a visual reference Ahri's orb in League Of Legends without wanting to recreate it exactly. The goal was to make a very beautiful visual effect without being optimized (the model uses more than 50,000 particles, which is not suitable for Video Games). So there are 3 layers of VFX that all use different workflows, that is: the first layer uses simple particles that are constrained in a sphere, the second is a simple particle that centralizes the effect and finally the "trails" are constrained at the surface of another sphere and make the orb irregular with a turbulence effect.

![Portal](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/VFX/Basis/TPortal.gif)

17/08/2022 : The portal effect seemed to me to be a classic among VFX Artists. This effect requires working on colors, timing and knowledge of work tools. To do this, I first had to create a circle texture on Photoshop. The shape of the portal may vary, but for the first time I decided to keep the circular shape. Then, each part of the final VFX was assembled according to a certain timing that had to be tested. The colors then came to intensify the atmosphere. The texture in the center was created by using a lot of knowledge from the Shader Graph, so I have a procedural texture.

![BeamAttack](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/VFX/Basis/BeamAttack.gif)

17/08/2022 : Another very popular effect that requires a lot more skills here especially in 2D: the Beam Attack (or Kamé Hamé Ha). To start the effect, you have to create a 2D Seamless Texture, that is, it can repeat to infinity without being noticed. It took many tests on Photoshop before having a result and then being able to use it. Then this texture is modified with the Shader Graph and then used in three different ways on the VFX Graph, to create three layers for the effect and give an impression of depth.

![Lightning](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/VFX/Basis/Lightning.gif)

16/09/2022 : This creation is quite important for me since it represents one of the pillars of what VFX Artists does, lightning. Although this one is generated procedurally without any texture, the speed of creation of this effect allows a certain optimization of the creation time. There is not much new to note for this effect. But the creation of this effect allows me to better understand the generation of 2D textures for lightning.

![Sword](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/VFX/Basis/Sword.gif)

22/09/2022 : A very cool effect that easily adds to many games and represents a huge satisfaction when the player uses it, the Fire Sword seemed to be a major reference. The creation of these VFX that compose this sword did not take more time than that since they had already been seen or worked before. We thus find a Shader to ignite the sword, a smoke that surrounds the sword and small ashes, themselves composed of a particle and a trail.

### Advanced (Done by my own with acquired knowledges, sometimes inspirations)

![Waterfall](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/VFX/Advanced/WaterfallShader.gif)

03/08/2022 : Many tutorials already offer to create their own Shader for liquid surfaces especially for water. So I decided to create mine with the Cell-Shading style as a reference (especially the Legend Of Zelda: Wind Waker). Using the same working techniques, I managed by testing different values and parameters to approach the desired result. The important thing here is the use of a Voronoï texture that allows this cellular aspect.

![MagicCircles](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/VFX/Advanced/MagicalInvocation.gif)

28/08/2022 : An effect that was very nice to create: the invocation circle. First, it was necessary to create the entire 2D textures, which proved to be much more complicated than expected (graphic bugs persist in the Unity version) but allowed me to use Photoshop in a deeper way. Then I had to create some animations and integrate them into the VFX Graph, which turned out to be simpler than expected. To finish everything rest on the timing of the appearance and disappearance of the different textures.

![Pokeball](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/VFX/Advanced/Pokeball.gif)

22/08/2022 : Taken from the Pokemon game, this effect is divided into 3 major parts that I had to understand and work on. First the modeling of the Pokeball and its animation. The animation was entirely made on Unity to make the most of the engine, while the model was made on Blender, as well as the materials to have a quick rendering. Then creating textures was also a challenge since, for example, dust clouds are mini-flipbooks. Finally the creation of the VFX were relatively simple, only the timings were tough to adapt.

![Blood](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/VFX/Advanced/BloodProcedural.gif)

10/09/2022 : The idea of this effect was to have a fast, simple and adaptable blood emission to any game. Here, we only use a default particle to simulate the blood but with a work on the texture, the blood can very quickly have a more realistic or cartoon style. Then, the working method of this VFX makes it possible to change very quickly where the blood comes from, to where, its emission frequency, and many other parameters, which makes this effect a real procedural effect when it used only the VFX Graph ( and the Shader Graph to improve blood rendering).

![Fireflies](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/VFX/Advanced/FirefliesFX.gif)

16/09/2022 : Fireflies are always a very good visual effect to add in a nighttime environment. These can have a behavior defined according to the player’s actions and add a more natural atmosphere to the game. They were made using Unity’s base particle system. Their random trajectory is obtained thanks to the added Noise after having obtained a pleasant result on the first iterations. Then their behavior is defined through a small script that understands whether the player is close or not.

![Explosion2D](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/VFX/Advanced/Explosion2DFbF.gif)

29/09/2022 : My first 2D effect took place over an entire week. It took a lot of testing especially on shapes and colors before I realized that the most complex was the timing. I started from simple forms that I gradually deepened. The explosion was an exercise that allowed me to gain a great experience both in 2D and in terms of timing, impact and understanding of VFX. The effect was entirely realized on Photoshop.

### Scenes (Works that are not only effects. Great artistic exercises)

![Sakura](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/VFX/Scenes/SakuraScene.gif)

![Sanctuary](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/VFX/Scenes/SnowSanctuary.gif)

![Witch](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/VFX/Scenes/WitchScene.gif)

![Esigelec](https://github.com/MatthieuAUBERT/MatthieuAUBERT.github.io/blob/main/Projects/VFX/Scenes/EsigelecOrder%231.png)

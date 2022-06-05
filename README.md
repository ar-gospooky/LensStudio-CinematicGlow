# LensStudio-CinematicGlow
Exponential glowing setup for Lens Studio that makes blooms/glows easy to set up.  
Works with multiple Cameras/Render Targets!

As seen in the Asset Library, and in [this tweet](https://twitter.com/gospookyhq/status/1533421429152264193).

The result looks better than Lens Studio's own Bloom asset, and it is better for performance (and more convenient to use) as it doesn't require you to make a duplicate of all the objects in your scene.  
However, this setup is slightly more complex and requires basic shader knowledge.

<br/><br/>

<img src="https://github.com/ar-gospooky/LensStudio-CinematicGlow/blob/main/Media/cinematic_glow.png" width="400">

<br/><br/>

A comparison between Cinematic Glow (left) and Lens Studio's Bloom asset.  
Cinematic Glow is brighter, and deals with thin glows better:  
<img src="https://github.com/ar-gospooky/LensStudio-CinematicGlow/blob/main/Media/glow comparison 2.gif" width="200">

<br/><br/>
  
# How to use
When the Cinematic Glow LSO is added to your project, create a new Render Target. This Render Target will be the combined render of your scene + glow.
<br/>
<img src="https://github.com/ar-gospooky/LensStudio-CinematicGlow/blob/main/Media/new_rt.png" width="400">
<br/><br/>
Let's give it a new name, like "Render Target + Glow".
<br/>
<img src="https://github.com/ar-gospooky/LensStudio-CinematicGlow/blob/main/Media/rename_rt.png" width="400">
<br/><br/>
Now, set this Render Target as the viewing target in Scene Config.
<br/>
<img src="https://github.com/ar-gospooky/LensStudio-CinematicGlow/blob/main/Media/set_rt.png" width="400">
<br/><br/>
Apply this Render Target and your scene's camera to Cinematic Glow.
<br/>
<img src="https://github.com/ar-gospooky/LensStudio-CinematicGlow/blob/main/Media/set_params.png" width="400">
<br/><br/>
You're done! From here on, you can make any material or VFX asset glow by accessing the 'Color Pass 1' input in it.
<br/>
<img src="https://github.com/ar-gospooky/LensStudio-CinematicGlow/blob/main/Media/color_target_1.png" width="400">


<br/><br/>

# Known issues
Post Effects overwrite Color Pass 1. This means that any Post Effects in the same Render Layer as glows will make the glows look off.  
Snap is looking into this, but in the meantime, try to place your Post Effects on a separate Render Layer.  
Or: see the workaround that's inside the 'Multiple Cameras Setup' example project file!

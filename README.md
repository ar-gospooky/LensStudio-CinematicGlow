# LensStudio-CinematicGlow
Exponential glowing setup for Lens Studio that makes blooms/glows easy to set up.  
Works with multiple Cameras/Render Targets!

As seen in the Asset Library, and in [this tweet](https://twitter.com/gospookyhq/).

The result looks better than Lens Studio's own Bloom asset, and it is better for performance (and more convenient to use) as it doesn't require you to make a duplicate of all the objects in your scene.  
However, this setup is slightly more complex and requires basic shader knowledge.

<br/><br/>
  
# How to use
When Cinematic Glow is added to your project, create a new Render Target. This Render Target will be the combined render of your scene + glow.
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

# Unity Simple Fade Camera
Fade your camera in and out to black/white or any other color, through a very simple shader, and postprocess script.

### Usage
- Add FadeCamera.cs and FadeCameraShader.shader to your project.
- Attach the FadeCamera script to your camera.
- you can now choose a color to fade in and out from in the inspector.
- You can then call the fade functions
```cs
//fade from color to camera in 1 second
cameraGameObject.GetComponent<FadeCamera> ().FadeIn (); 
//fade from camera to color in 1 second
cameraGameObject.GetComponent<FadeCamera> ().FadeOut (); 
//fade from color to camera in 5 seconds
cameraGameObject.GetComponent<FadeCamera> ().FadeIn (5f); 
//fade from camera to color in 5 seconds
cameraGameObject.GetComponent<FadeCamera> ().FadeOut (5f); 
```
 if you want more control over the fade animation, you can use the `.opacity` and `.color` properties and lerp it as you please.
 
 You check the example scene for usage.
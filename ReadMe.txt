This asset contains a simple script to emulate a lip sync for a virtual agent. Why did i do that? Because of the lack of free lip sync assets for Unity, but of course! I got most of this code online and adjusted to what i needed for. Then, tried to make it the most general possible, so it would be easy to integrate for others. It may not be the best or the most accurate lip sync tool, but it is free and easy to use =)

HOW TO USE:

Download and import the asset into your project. You will see that it counts with a LipSync.cs script. Add this script as a component of the GameObject that you want to use. Fill the fields that you will need and you are done. Pretty simple uh? Next, i present some important details of this configuration.

- In which gameobject should i add the script component? It will depends on the mesh you have as your virtual agent, especially concerning the mouth. In general, there are two ways used to animate mouths: Jaw Movement and BlendShapes. Jaw Movement is the simplest one, since it only needs the mouth itself. This asset counts with a virtual agent based on Jaw Movement, so you can use it as an example. Blendshapes are more complex, but deliver a better and more fluid animation. If your agent uses Blendshapes, you should add the LipSync script as a component of the object which contains the definition of the blendshapes. Otherwise, if you have a simple jaw, you should add the LipSync script as a component of the mouth object (in this case, you can use the agent of this asset as an example).

- The gameobject which receives the script must have an AudioSource component, because it is from where it gets the audio used for the lipSync. For the blendshapes, it also needs to have a SkinnedMeshRenderer with the blendshapes.

- When the script is added, you can see that it has some parameters. If your model is based on Jaw Movement, you only need to mark the Is Jaw ticket. If your model is based on blendshapes, untick the Is Jaw ticket and inform the index of the blendshape which deals with the mouth movement, in Bs Index.

- In the script, the Aperture parameter controls how much the mouth open. The higher the value, the less the mouth opens. If you think yours is opening too much (or too little), you can change this value and test which is the best for you.

That is it. If you have any question or whatever, just send a message =)
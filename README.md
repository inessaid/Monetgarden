# Monetgarden
![facing pagoda](https://user-images.githubusercontent.com/43462511/110391964-39213900-8036-11eb-8ff6-88173bbb80bb.JPG)

## Inspiration
At some point, everyone gets overwhelmed with their day to day routine. Whether it be sitting in the office, pencil-pushing paperwork or taking care of the (never-ending) chores at home, life always manages to find a way to wear us out. Today, its even harder to take the necessary steps for self-care when things get tough, thanks to COVID-19 being an ever-present, extremely stressful factor in everyone's life. 

We wanted to find a way to help individuals get the self-care time they need in a world which is locked up, put indoors and endlessly stressful. Looking back on our own experiences, our team realized that the beautiful public gardens which we miss so much would be the PERFECT place to do this. So we set out to recreate one of life's finest luxuries in as realistic a way as possible (and you don't even have to put on a mask!). That's how we got started on Monet's Garden!
 
## What it does

Monet's Garden is a public garden with a twist; your own personal self-care assistant! Monet's Garden offers guided meditation, beautiful views for a relaxing virtual walk in the park, and a unique opportunity for recreation- light painting! 

You can enter the application from the office, school, or even at home, and be instantly transported to a lush public garden with broad walking paths, a bamboo forest, and a pergola for guided meditation! If you walk up to the pergola,  you will begin to hear a soothing voice which guides you through a short session of relaxation and meditation, focusing on self-acceptance and care towards yourself and others. After that, you can enjoy the variety of natural resources we've polished in Monet's Garden! The majority of our assets are photogrammetry models, meaning they are photorealistic replicas of real-world objects imported into our virtual garden-- so you really can have the best of both worlds. Last, but certainly not least, if you're feeling like some more active self-care activities to relax and de-stress, you are able to light paint throughout the gardens. Exercise your creativity while forgetting your troubles!

## How we built it
**Lighting**
We used this hackathon as an opportunity to learn and experience some of the newest lighting features of the latest Unity update. We used multiple local volumes to have a personalized lighting effect within different areas of the environment. Increasing the fog levels and the volumetric multiplier also allowed us to simulate volumetric lighting passing through and around the transparent foliage in the environment. 

Marking stationery items such as the rocks or stone to static lets the Unity Lighting system recognizes which objects can receive any baked lighting. The combination of the baked lighting and baked reflection probes heightens the fidelity of the environment without using real-time performance draining lighting.

Post-processing overrides on the sky and fog volume of the scene also enhanced the overall aesthetic of the environment. Overrides such as bloom, vignette, tint, and screen space ambient occlusion were some of the contributing factors of environment beautification. 

Light Proves found within the scene allows for the proper change of light bounces as non-stationary assets move through the environment, such as the user.

**3D Modelling**
One major attraction in Monet's Garden is the beautiful natural environment we've prepared for our visitors! We leveraged the Unity HD Render Pipeline together with the Quixel Megascans library to create a photorealistic environment comprised primarily of photogrammetry models. We also used resources prepared by Unity for the HD Render pipeline in order to further develop our environment. 

We started by developing a landscape design plan, as informed by the University of Florida IFAS extension guide on real-world landscape design. After developing a plan, we modelled basic assets in Maya, including the pathways and bridge assets. This allowed us to exercise greater flexibility with our composition than we would've been able to with standard terrain tools. After establishing our basic shapes, we began to develop set-pieces, largely using Quixel assets like rocks, small trees, and plants. At this time we also began to work on lighting, which was a major component of this scene (as described above). After building landmarks and blending shapes, we began to fill out the scenes smaller details like ground cover, particle effects and distant forest details. Finally, we began to structure the terrain to include water resources. At that point, the scene was practically finished. 

**VR Interaction**
We used unity to create the virtual reality environment. The main programming language used is C#. We used the Unity Oculus Integration package to allow for interaction within the environment. The player can walk around the trails of the environment either using the controller or by walking around an empty room. We used particle systems and hand tracking to create the virtual drawing light effect. the particle systems have a set lifecycle and they’re smoothed out to leave a glowing trail wherever the user moves their hands. We also used particle systems for the butterflies and the glowing dust around the scene. 

## Challenges we ran into

Working with complex environment scenes is challenging, both for the computer and for the artist behind it. Our first issue was dealing with bugs and incompatibilities between the Quixel Megascans library and the Unity HD Render Pipeline. We had to manually convert all textures into HDRP textures, and many plants simply would not work. This unfortunately limited our choices of foliage to a certain degree. The HDRP in Unity 2020 furthermore lacks broad-scale support for water shaders, which posed a significant challenge to our ability to deploy water in the scene as we saw fit. Finally, we used the Oculus Quest 2 for the first time, which required configuring and troubleshooting before working properly with the scene. We weren't quite sure if the Quest could handle scenes developed in the HDRP, but we were pleasantly surprised to find the device was significantly stronger than we anticipated. The only major problem we had with it was higher-than-usual levels of motion blur, which was at most a minor annoyance.  
(The project is too big to be fully put in github. We were only able to put a partial part of our project in our github repo.)

## Accomplishments that we're proud of

First and foremost, we are proud to have built a 3D environment in less than 2 days which is beautiful, functions properly, and is as large scale as we were able to make it. The Unity HDRP is exciting for any virtual artist, and being able to take advantage of it in this project was a pleasure. We also got to build out an extensive scene with Quixel Megascans for the first time; we had never before attempted a project as large as this one. Lastly, we were proud to have worked on something new together, as many of our team members have not worked on similar projects before. Participating in Hack Violet was a learning experience which was well worth the effort. 
This is also our first project ever using Oculus Quest 2! It was really exciting to play with this news devices but it also came with its own challenges! 


## What we learned

Our team was able to significantly deepen our knowledge of Unity and the HDRP through this project. While most of us had experimented in some way with it, none of us had ever built as scene as robust as this one. Developing the landscape design, lighting, texturing, and working with the 3D models for the project was a large task (for which we have not yet slept), but it was a learning experience which we will certainly carry forward into the future. 
We learned how to optimize HDRP environments for Virtual Reality, specifically for the Oculus Quest 2. We also learned how to upgrade the texture from standard to HDRP. 
Several of us never used particle systems before and it was fascinating to learn how to draw in the air with sparkles of lights! We can see so many future use cases for that and we can’t sit to develop them in further Hackathons! 

## What's next for Monet’s Garden

The next step for Money’s garden is to provide customization of the environment. We briefly tried to work on that during the hackathon but there wasn’t enough Time to finish it. We’d also love to provide different scene options where the user chooses their favorite environment to meditate, and also choose from different guided meditation tracks. 

![bridge](https://user-images.githubusercontent.com/43462511/110392338-c6fd2400-8036-11eb-914c-a5eb4b2734f2.JPG)
![pond](https://user-images.githubusercontent.com/43462511/110392348-cd8b9b80-8036-11eb-8102-8707500b38ad.JPG)



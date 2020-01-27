+++
# Date this page was created.
date = 2018-11-10T00:00:00
layout = "project"

# Project title.
title = "1. Expedia Project"

# Project summary to display on homepage.
summary = """
This is a study abroad project that took place in Vienna, Austria. <br>
My group collaborated with an Austrian Semantic Web Company who wanted to establish a long-term partnership with Expedia. My group built cognitive Artificial Intelligence solutions to help the clients from Expedia enhancing the user experience of low vision travelers in Austria.<br>
 """
 
image_preview = "expedia.jpg"

# Tags: can be used for filtering projects.
# Example: `tags = ["Computer Graphics", "Rendering"]`
tags = ["Computer Graphics","Rendering"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# [header]
# <<<<<<< HEAD:content/project/1 expedia/index.md

# image = "img/expedia.jpg"
# =======
# image = "expedia.jpg"


+++

# Overview
This project aimed to help the clients from Expedia by building an AI knowledge Graph to enhance the experience of low vision travelers in Austria. During the project, my group mates and I organized and extracted data from open-source database and delivered data to users’ phones or tablets.<br>
I took the roles of user experience researcher and prototype designer. <br>

The main accomplishments carried out by my groups are: <br>
1. Created user personas, user scenarios, and knowledge graphs to identify the needs, goals, and behaviors of low vision travellers. 
2. Built an AI knowledge Graph to enhance the experience of low vision travelers using Expedia. <br>
3. Developed a whole set of taxonomy and ontology using PoolParty Semantic Suites and connected content from Google Maps, Municipal Data, and other open-source data such as Wikivoyage to expand the database.<br>
4. Used SPARQL Queries to extract data from open-source database and delivered data to users’ phones or tablets.

# Features
## User Research

### Personas (Fictional representation of our typical customer)

In order to identify the needs, behaviors, and goals of our target users, my group created some user personas (Fictional representation of typical customer) to narrow the scope of our project. 
![Linda](img/Linda.jpg)
![Frank](img/Frank.jpg)

Then, I Improved it to support more shaders, such as texture mapping and interpolating parameters.
![Shaders](img/Shaders.jpg)

To render complex scenes, I added a heuristic bounding volume hierarchy (BVH) to store the primitives in an efficient manner. Also, I optimize the sphere and triangle intersection routines. In most scenes, the speed of rendering has been accelerated by more than 50x.
![Test Scene 1](img/BVH.jpg)
A complex scene rendered within 2 minutes:
![Test Scene 1](img/Scene2-Test5.jpg)

Now, it is the time to implement path tracing!

## Monte-Carlo integration & Path Tracing

To support pixel antialiasing, I implemented a box filter over the pixel footprint and depth of field by integrating over the aperture of the camera illustrated as follows:
![Antialiasing1](img/Antialiasing1.jpg)

As for the depth-of-field effect, I simulated an imaginary thin lens with a fixed aperture to produce a nice depth-of-field effect, where some objects will be sharp but others blurry.
![DepthOfField1](img/DepthOfField1.jpg)

Original scene:
![Test Scene 1](img/Scene2-Test4.jpg)

Depth-of-field effected scene:
![Test Scene 1](img/DepthOfField.jpg)

Now, here is the most important part! 
A basic Monte-Carlo estimater was implemented to sample radiance of the hemisphere.
![Test Scene 1](img/PathTracing.jpg)
By integrating the radiance coming from the hemisphere, we could estimate the radiance of indirect illumination. So far, we can get the global illuminated scenes as follows.
![Test Scene 1](img/PathTracing2.jpg)

## Final thesis

Also, I added a basic volumetic scattering effect estimater in this path tracer and wrote a final paper in SIGGRAPH tamplate which discussed principles of volumetic rendering and path tracing.

![Test Scene 1](img/Final1.jpg)
![Test Scene 1](img/Final2.jpg)
![Test Scene 1](img/Final3.jpg)
![Test Scene 1](img/Final4.jpg)
![Test Scene 1](img/Final5.jpg)

For more information and source code: https://github.com/XiangmingKA/PathTracer
![Test Scene 1](img/Scene-Test4.jpg)


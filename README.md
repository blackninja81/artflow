
 # Artflow: Blender-to-Three.js Visual Buildings

Welcome to ArtFlow, a project for designing visual buildings in Blender, rendering, and integrating them into a Three.js environment using WebGL

## Prerequisites

- [Blender](https://www.blender.org/) (version 2.8 or higher)
- Node.js and npm
- Gits

## Getting Started

To run this project locally, follow these simple steps:

1. ```git clone https://github.com/blackninja81/artflow```
2. cd artflow
3. Open the project in your preferred code editor.
4. In the Terminal, install npm by running the command ```npm install```
5. To view the project in browser, run the command ```npm run dev```

## Usage

Design your building in Blender.
Render the model in Blender.
Export the model as GLTF format.


## Blender Setup
 Open Blender and load your building model.
 Adjust camera angles and lighting for optimal rendering.
 Export the model as GLTF format.

 ## Blender
 - We used Blender to deal with creating the 3d model first we created the basic layout of the model using various components such as cubes and plesh. 
 - We used a third part addon (poliion) to add various furniture across the room. 
 - We used poliion to add textures to various surfaces.
 - We also used xoio 3D people collection to add humans to our model.
 - Due to the size of the project we had to cut out some features and objects due to very high render times and hardware limitations. 
 - Using Three.js to display this 3D model on the web allowed us to showcase our work interactively. 

 ## 3js
 - We exported the complete model using to gltf format to be able to handle it in threejs. We built the app on react framework
 - We used the following dependencies: 
 - @react-three/fiber @react-three/drei you can install them using ```npm i  react-three```
 - On importing the model we ran the following command to generate a 3js file for the model ```npx gltfjsx public/name.glb```                                                          
 - This creates a file Name.jsx which contains the 3js cordinates. 
 - From here we imported the file into the App.jsx file and setup the canvas for the 3js model. In this file we also defined 
 the controls to move the camera around as well as the mouse.
- We then run the command ```npm run dev``` this runs the web app in the browser. The web app experiences some render issues 
 therefore some items may appear and dissapear depending on the camera perspective.

## Project Backed Up to Google Drive
- Given the large size of the assets we are using google drive to store them
- After cloning the repo download the public folder from the drive link  below. Paste it into the project replacing the current public folder
- Run npm install to install all necessary dep`endencies
- Link: https://drive.google.com/drive/folders/1lK8XBYA7f4x3PoAzf01W1xgiogZG6ltW

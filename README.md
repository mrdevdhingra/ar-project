# AR Camera Experience

A Snapchat-like AR web application that displays 3D models when scanning specific markers.

## Features
- Mobile-friendly camera interface
- Marker-based AR using AR.js
- Interactive 3D model display
- Click interaction with models

## Setup

1. You'll need to add two files in the `assets` directory:
   - `pattern-marker.patt`: The AR.js marker pattern file
   - `scene.gltf`: A 3D model in GLTF format

2. To generate your own marker:
   - Visit https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html
   - Create your marker
   - Download the pattern file and save it as `assets/pattern-marker.patt`
   - Print the marker image for testing

3. For the 3D model:
   - Use any GLTF format 3D model
   - Save it as `assets/scene.gltf`
   - Make sure to include any associated files (textures, etc.)

## Usage

1. Host the project on a web server (required for AR.js to access the camera)
2. Open the website on a mobile device
3. Allow camera access when prompted
4. Point the camera at your printed marker
5. The 3D model will appear above the marker
6. Tap the model to see the "Hello there!" message

## Technical Requirements
- Modern mobile browser with WebGL and camera support
- HTTPS connection (required for camera access)
- Stable internet connection

## Development
The project uses:
- AR.js for augmented reality
- A-Frame for 3D rendering
- Vanilla JavaScript for interactions 
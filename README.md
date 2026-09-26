# Sound Reactive Bubble

An interactive browser-based audio visualization built with JavaScript and p5.js. The application captures microphone input and uses the incoming audio level to dynamically alter the size and shape of a 3D wireframe bubble.

## Launch Website

[Open the Sound Reactive Bubble](https://landonbotelho.github.io/soundReactiveBubbleWebsite/)

> Microphone permission is required for the audio-reactive functionality.

## Overview

The visualization renders a rotating 3D mesh that reacts in real time to microphone input. Audio amplitude controls both the overall size of the bubble and the intensity of its surface deformation.

The surface is generated from spherical coordinates and modified using multiple layers of Perlin noise to create smooth, organic movement.

Users can also rotate the visualization interactively with the mouse.

## Features

- Real-time microphone input using `p5.AudioIn`
- Audio-driven mesh deformation
- 3D rendering using p5.js `WEBGL`
- Perlin-noise-based surface distortion
- Dynamic bubble scaling based on audio amplitude
- Smooth microphone input interpolation
- Mouse-controlled 3D rotation
- Responsive full-screen canvas

## Technologies

- HTML5
- CSS3
- JavaScript
- p5.js
- p5.sound
- WebGL
- Web Audio / microphone input

## How It Works

The bubble is constructed from a series of rings and slices distributed across a sphere. Each vertex begins at a position calculated using spherical coordinates.

Two layers of Perlin noise are then applied to modify the radius of each vertex, producing the uneven organic surface.

Microphone amplitude controls:

- the overall radius of the bubble
- the magnitude of the Perlin-noise deformation

As the detected sound level increases, the visualization grows and becomes more distorted.

## Running Locally

Open `index.html` in a modern browser and click **Start Audio**.

For microphone access, the page may need to be served through HTTPS or a local web server depending on the browser.

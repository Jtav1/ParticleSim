# ParticleSim
Web browser particle simulation exercise

## Usage
By default, the simulation shows a snowfall. Click the blue and white buttons to switch between Rainfall and Snowfall, respectively.

* Click the simulation to pause
* The Windspeed slider contrls the horizontal "wind" force on the falling particles. Snow is lighter than rain.
* The Particle Density slider controls the chance that a new particle will spawn on any given refresh of the simulation (currently hardcoded to 30ms).
* The Gravity slider controls the force of "gravity" pulling the particles towards the ground. Negative gravity is not an option, we haven't invented that yet.

## About the Implementation
### How to run ParticleSim
Open ParticleSim.html in your web browser. The implementation is entirely contained within that file, and has been tested for compatability with current builds of Chrome/Firefox/Edge.

### Design choices

* ParticleSim contains functions for creating Particles and Buttons, which should allow for ease of adding new particles and buttons to select them.
* Sliders were a creative liberty, I wanted to see if I could effectively change the properties of the simulation "world" on the fly. Plus, I didn't know how important it was to demonstrate that the snowfall falls AND blows. 
  * Note that particles only spawn from the top of the simulation, not outside. Particles can be blown off the canvas, but new particles will not be created off-canvas and blown onto the canvas. 
* Gravity is factored into the wind force on the particles, such that when gravity is turned up the "wind" still seems to have an effect.


### Why ParticleSim?
I had no idea how to start this project, so I picked it because it put me the furthest outside my comfort zone :) I feel like I have a rough idea how to do the other two exercises - A Java OCR library like Aprise and some regex, or a tree of word beginnings and endings for the keyboard.  

While I have worked in web development professionally, I haven't had a chance to play with some of the newer HTML5 features - I felt this was a good reason to learn about HTML5's Canvas.


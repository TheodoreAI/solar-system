# Project Proposal for Hackathon 4

## Summary

- To simulate the orbit of Mercury using three.js, Newtonian orbital mechanics, and general relativity

## Goal

- The following application uses three.js to simulate the Sun and Mercury using Newtonian physics to get the orbit of Mercury, simultaneously simulating the perihelion shift of Mercury with General Relativity. The user will be able to navigate the environment using their mouse, the user will also be able to see the difference in the orbital angular velocity given the two different orbital periods.

## Location

- My own repo

## Requirements

- create vue3 project and install threejs
- integrate threejs to vue3
- Create a scene
- initiate the scene
- create the Sun
- Create a light source at the center of the sun
- create a mesh with the geometry of the sun/mercury and the images
- create mercury as a planet
- give mercury a rotation about its own axis using rotateY
- give mercury an orbit around the sun that is not circular but instead has an elliptical rotation:
- stretch give mercury an orbit around the sun that takes into account the perihelion shift

- VueJs3 front-end

## Proposed Approach

- [Solar System Demo](https://www.youtube.com/watch?v=KOSMzSyiEiA)

## Technologies

- Vue3 Bootstrap Boilerplate v2.0.0
- [Three.js](URL here)

## Directory structure

```bash
cem-263-leveling
├─ src
│ ├─ App.vue
│ ├─ components
│ │ ├─ template.vue
│ │ ├─ activity
│ │ │ └─ SolarSystem.vue # component with drawing.js
│ ├─ js
│ │ └─ three.js
│ └─ views
│ └─ Main.vue # Where the component be rendered
```

## Proposed State

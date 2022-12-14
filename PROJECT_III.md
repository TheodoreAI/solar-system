# Project Proposal for Hackathon 4

## Summary

- The following application uses the JavaScript library three.js to simulate the solar system which includes the Sun and it's nine planets

## Goal

- To simulate an interactive solar system using three.js that can pass data between the threejs canvas and the vue front-end

## Location

- My own GitHub repo: solar-system

## Research - howto
- integrate threejs module with a Vue component
- initiate a scene
- create a light source
- create meshes with images and an object
- [Threejs](https://threejs-journey.com/lessons/3#)

## Requirements

- Vue application that can import threejs
- integrate Threejs to Vue - two way communication between the two (probably using callback to pass an object with the necessary data)
- Have a solar system scene
- Need a light source at the center of the sun
- Planets
- first four planets
- give planets a rotation about their own axis using rotateY
- give planets an orbit around the Sun that is circular
- Stretch: do all nine planets

## Proposed Approach

- [Solar System Demo](https://www.youtube.com/watch?v=KOSMzSyiEiA)

## Technologies

- Vue create app
- [Three.js](https://threejs.org)

## Directory structure

```bash
SolarSystem
├─ src
│ ├─ App.vue
│ ├─ components
│ │ ├─ template.vue
│ │ ├─ activity
│ │ │ └─ PlanetScene.vue # component with drawing.js
│ ├─ js
│ │ └─ three.js
│ └─ views
│ └─ SolarSystem.vue # Where the component will be rendered
```

## Proposed State

```JavaScript
data(){
    return {
        planetData: {Mercury: [], Venus: [], Earth: [], Mars: [], ... };
    }
}

// To get data from threejs
let callback: function (dataStructure)=>{
    let planetData = dataStructure.planetData;
}

function method: {
    three.sendCallback(callback);
}

// To send data to threejs
three.sendDataStructure(planetData);

```

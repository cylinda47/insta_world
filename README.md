# InstaShow - an Instagram feed visualization

## Background and Overview

InstaShow is an interactive tool that allows user to click on anywhere on a spinning globe on one side, and get an instant live feed of photos on the other side.

## Functionality & MVP

In InstaShow, users will be able to:

- [ ] Click on any country/city from a spinnable colored globe, and
- [ ] Get a grid of most recent photos
- [ ] Get push update from Instagram subscription and display new photos in that location
- [ ] Photos re-sorting animations whenever there is a new photo feed

## Wireframe

This app will consist of two parts - a map/globe simulation and a grid of live photos.

![](https://github.com/cylinda47/insta_show/blob/master/wireframe.png)

## Architecture and Technologies

This project will be implemented with the following technologies:

* Vanilla JavaScript for overall structure and game logic

* `node.js` for backend request handling
* `D3` for data visualization
* `topojson` for generating topology
* `Instagram API` for querying photos based on location & get push updates
* `Webpack` to bundle and serve up the various scripts.

In addition to the webpack entry file, there will be four scripts involved in this project:

`main.js`: this script will host the following files and handle the interaction between them

`topology.js`: this script will handle the logic for topology stimulation.

`photos.js`: this script will handle .

## Implementation Timeline

**Over the weekend:**

- [X] Complete `d3` and `topojson` tutorials

**Day 1: Topology**

- [ ] Setup all necessary Node modules, including getting webpack up and running.
- [ ] Start creating a basic topology using `topojson`
- [ ] Load map data using `d3`

**Day 2: Instagram data**

- [ ] Style the globe
- [ ] Import photos using `instagram API`
- [ ] Enable search query based on latitude and longitude

**Day 3: Topology Integration with Instagram data**

- [ ] Enable ajax request to Instagram server with the location parameters when user click on a selectable part of the globe
- [ ] Display the incoming photos

**Day 4: Live feed from location**

- [ ] Setup the node server for receiving Instagram subscription
- [ ] Append incoming photos to the frontend page

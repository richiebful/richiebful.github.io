---
layout: post
title: Adventures in front-end development
category: work
---

I've never really made a JavaScript app. Frontend...it's just not something I've gotten into. I've added a little functionality here and there with JS, but mostly just to make a static page do something a little bit special. No sweat. But JS makes it really easy to write spaghetti code and modularize nothing. It's not a problem when you're just drawing a few things on a canvas or handling a small amount of user input in isolation. But then I started working on my farmplot app. Heaps and mounds of spaghetti code.

I started off extending Leaflet.js with a drawing library (Leaflet.pm), by writing functions above my window.onload event handler. Bad idea. Before long, I ended up with a pile of global variables and little idea of where I was going. But thankfully, the Leaflet plugin I was using has a solid modular design. I dug into the source code and quickly learned how I could apply some of my OOP tricks to JavaScript.

I quickly made classes for geometric Features, so I could compare them and add non-geographic properties, like “How much pH was read at this marker?”. Then I made a List to contain these Features in. Using this construct, I can click on the Leaflet marker on the map, type in that pH data, and update the backing data for these markers, even on disk in GeoJSON format. I also learned that dividing my JavaScript project into multiple files and compiling into one JS file at the end makes a whole lot more sense. In other words, time to learn gulp.

In short, lesson learned: if a coding practice is leading you to the point where you have a steaming mess of code, it's time to do some research. Ask a senior programmer. Use the internet and find a mature JS project. Don't ignore that gut feeling that something is wrong. Something probably is wrong, and it can be fixed.
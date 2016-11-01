# Hello
## I'm Max Glenister

---
### omgmog.net
### blog.omgmog.net
### @omgmog elsewhere

---
## UX/Front-end Developer
### Aris Technologies
#### \(we make online casino games)

---
## Web designer/developer
### Marmalade & Jam
#### \(we mostly make websites for pubs)

---
## I like to
## dabble with VR

---
![](images/CUHjrioWsAQq0On.jpg)
### 20 minutes into the future
###[fit] with Google Cardboard and JavaScript
#### Watch it here: https://git.io/vXtu3
^ I gave a talk this time last year called "20 minutes into the future", where I explained how you can use JavaScript to make Google Cardboard experiences

---
![](images/uxofvr.png)
## UX of VR
### www.uxofvr.com
^ I created UXofVR.com -- a curated list of articles and resources for learning/applying good UX in your VR projects.

---
![](images/CoCXiyCXgAATON1.jpg)
## Game Dev Day
### Summer of Hacks 2016
^ For the JS Oxford Summer of Hacks, I organised Game Dev Day. I encouraged people to create VR hacks using A-Frame

---
## After that...
^ I was looking for another VR project to work on

---
## And then in September
^ Then in September, Ben Foxall sent me a message on the Digital Oxford Slack

---
# ...

---
![inline fit](images/Chat.png)

---
![inline fit](images/Chat Copy.png)

---
![inline fit](images/Chat Copy 2.png)

---
![inline fit](images/Chat Copy 3.png)

---
![inline](images/google-cardboard.png)
# Cardboctober
^ So the idea of Cardboctober was born

---
## 31 days
### of making things
### for Google Cardboard
^ The plan was simple

---
![](images/easy.gif)
## **EASY MODE**
### **join in sometimes**

---
![](images/regular.gif)
## **REGULAR MODE**
### **join in every day**

---
![](images/hard.gif)
## **HARD MODE**
### **all of above & blog daily**

---
## I made some
## cool things...

---
![inline fill](images/giphy-06.gif)![inline fill](images/giphy-08.gif)
![inline fill](images/giphy-09.gif)![inline fill](images/giphy-10.gif)
![inline fill](images/giphy-11.gif)![inline fill](images/giphy-13.gif)

---
## And so did
## other people

---
![inline fill](images/pete-06.png)![inline fill](images/pete-15.png)
![inline fill](images/pete-17.png)![inline fill](images/pete-20.png)
![inline fill](images/pete-26.png)![inline fill](images/pete-27.png)

>By @peterjwest

---
![inline fill](images/ben-02.png)![inline fill](images/ben-03.png)
![inline fill](images/ben-05.png)![inline fill](images/ben-06.png)
![inline fill](images/ben-09.png)![inline fill](images/ben-16.png)

>By @benfoxall

---
## Check them out
### cardboctober.xyz

---
## It was a
## lot of work...

---
## How did I do it?

---
## Lots of<br>Planning
^ Well, for me it began with a lot of planning...

---
### Week 1
## Basic VR

---
```html
<html>
  <body>
    <script src="three.min.js"></script>
    <script src="basic-vr.js"></script>
  </body>
</html>
```
---
```javascript
// Setup the camera, renderer, scene, etc.

// Make a cube
var geometry = new THREE.BoxGeometry(1, 1, 1);
var material = new THREE.MeshBasicMaterial({color: 0xff0000});
var cube = new THREE.Mesh(geometry, material);
scene.add(cube);
```
---
```javascript
// Called 60 times a second using rAF
var update = function () {
  cube.rotation.x += .1;
  cube.rotation.z += .1;

  renderer.render(scene, camera);
  requestAnimationFrame(update);
};

// Call it once to begin
update();

```

---
# Here's one I made earlier
![inline](images/basic-vr.gif)

---
## But Max<br>that's not VR
### That's just a spinning cube!

---
```html
<html>
  <body>
    <script src="three.min.js"></script>
    <script src="StereoEffect.js"></script>
    <script src="basic-vr.js"></script>
  </body>
</html>
```

---
```javascript
// After setting up your renderer
effect = new THREE.StereoEffect(renderer);
effect.eyeSeparation = 1; // Set the IPD
effect.setSize( width, height );


// Instead of calling renderer.render(scene, camera)
effect.render(scene, camera)
```

---
![inline](images/basic-vr-stereo.gif)

---
#[fit] :boom: :package: 🕶 :boom:

---
#[fit] I also covered
#[fit] some other things...

---
- Raycasting
- Skyboxes
- Mesh generation
- Using .stl models
- Creating a "match two" game

---
### Week 2
## Web APIs

---
// speech recognition, audio

---
### Week 3
## UX of VR

---
// fullscreen for an immersive experience, moving around, hierarchy of needs

---
![inline](images/hierarchy1.png)

---
![inline](images/hierarchy2.png)

---
### Week 4
## Tetris in VR

---
// good week-long project
// skills we've picked up over cardboctober
// 2-dimensional array manipulation
// collision algorithms

---
## What have
## I learned?

---
// stuff
// save time by factoring out common boilerplate to save time
// test often, test on other people
// you're not creating AAA games every day, so don't worry about making it perfect
// if you're learning from it, others can too

---
## Pros

---
### Force yourself to learn something new

---
### Great for content creation

---
### Github commit streak

---
## Cons

---
### Takes a lot of time

^ 2-3 hours per day

---
### Be considerate of
### your loved ones

^ My wife had to listen to me talk about VR non-stop for a month

---

## Closing thoughts

---
// stats
// - - max/ben/pete
// - commits
// - lines of code

---
## Questions?


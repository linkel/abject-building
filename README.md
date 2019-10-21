# What's this?

I'm playing around with the matter.js engine. I painstakingly put together a person's body on the canvas. Seriously, it took longer than I thought! The documentation for matter.js is a little opaque.

You can drag him around and throw things at him. 

# The meat

This was like a little art project. Decided that I wanted to make shapes for each body part and used [constraints](https://brm.io/matter-js/docs/classes/Constraint.html) (which are like springs that you can adjust to be more rigid or more elastic with damping or not) to connect the body parts together. 

As far as I can tell, matter.js seems to be able to hook into a canvas html object. If you don't specify one, it makes one on its own. If you specify one, you can tweak the size by providing configuration information in the form of an options object to the Renderer. All physics objects made need to get added to the World, then you can run the engine to initialize it all.

![dude](./matter_exp.png)

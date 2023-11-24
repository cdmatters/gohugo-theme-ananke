---
date: 2015-03-09T10:58:08-04:00
description: "an almost familiar game" 
paragraph: "a 400-line javascript implementation of snake in polar coordinates"
featured_image: "/images/snayk.png"
tags: ["javascript", "interactive"]
title: "snayk"
---


snayk is a game in 400 lines of pure javascript, written during my time at [the Recurse Center](https://recurse.com). It is simply the classic game of snake, adapted to use polar coordinates, instead of Cartesian ones. You can play snayk [here](/snayk).


### Background

I had just finished my physics degree at Cambridge, and had already spent some time thinking about how different coordinate systems can make problems easier or harder. 

While at RC, I attended a seminar run by [Mary Rose Cook](https://maryrosecook.com/) in game development, in which she laid out the basics of coding up Space Invaders, based on her very popular [annotated code blog posts](http://annotated-code.maryrosecook.com/). 

In the seminar, I decided to make a version of snake in polar coordinates, and my code follows that architecture closely. It was my first javascript project.

### Polar Coordinates

In polar coordinates, the locus of points is described by distance from a central point \\(r\\) and an angle \\(\theta\\) from a reference direction (normally the \\(x\\) axis).  This contrasts with Cartesian coordinates (\\(x, y\\)), which describe points by their distance along the \\(x\\) and \\(y\\) axes. 

In Cartesian coordinates, the basic 'directions' of motion are:

* Up, Down, Left and Right. 

In Polar coordinates, the basic 'directions' are: 

* Away (from Centre), Towards (Centre), Clockwise, Anti-Clockwise. 

In principle, all problems can be solved in either coordinate system - but the tidy analytic solution may only exist in one coordinate system. 

For instance, orbital mechanics is very simple and elegant in polar coordinates, but a mess in cartesian coordinates; for projectile mechanics, the opposite is true. 


### Stack

* javascript

### [Github](https://github.com/cdmatters/snayk) | [Play](/snayk)
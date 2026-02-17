# Java Game Development

This repository contains the source files for [a tutorial series](https://majicktek.github.io/javagamedev/) on game development in Java.

## Goals
The end result will be a 2D game engine that is modular and is designed to have plugin/mod support from the ground up. This means it will be very easily customizable, and each part of the codebase will live by itself and be small/understandable. No monorepos!

Many Java game development series use the same kind of single-threaded basic AWT renderer, but the end goal is to have this be far more capable and hopefully support both software and hardware rendering.


## Tasks
* Design a stable API
* Create a base program that will allow selecting the engine implementation modules (such as backend renderer), as well as "third party" extension plugins (mods)
* implement one or more types of "base" plugins.
  - renderer
  - sound engine
  - physics engine
  - entity system
* Once enough of the base is implemented, there should be a playable game to go with it.

## Tech
* possibly Raylib as a backend, this will map nicely
* high level UI implementation, built using the engine's renderer API
* Some Java-based and game-focused sound library
* ECS for the entity system
* Pure Java physics? Should I implement this by hand or use an existing library? probably the latter
* I want to possibly use [Resource Handles](https://giordi91.github.io/post/resourcesystem/)
* Have some kind of event system t=with scheduled events, maybe tick based. game/render/physics loops can be sparate
* Introduce basic networking?

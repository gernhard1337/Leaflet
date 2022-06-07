
# TABLE OF CONTENTS

1. [INTRODUCTION](#introduction)
2. [USER JOURNEY / PROGRAMMERS ASKS](#Requirements)
   1. [User Requirements](#user-requirements)
   2. [Programmer Requirements](#programmer-requirements)
   3. [technical Requirements](#technical-requirements)
3. [Stakeholder](#stakeholder)
4. [View](#view)


## INTRODUCTION

The aim of Leaflet is to provide a simple, performant, lightweight JavaScript-Library to enable a simple handling 
for interactive Maps. 
This Document defines severall Requirements that shall be satisfied by Leaflet. 
Those Requirements are created by Reengineering since Leaflet has no Requirement Table till Version 1.8.0 and only 
provides Documentation about the API for Devs.

----------
###What is leaflet JS? 

Leaflet is a well-known open-source JavaScript framework that allows developers to add lightweight, simple, and interactive geographic maps to any website or project in an elegant way.


###leaflet main functionalities in a nutshell.

-	Creating lightweight maps in a simple readable code.
-	customizability with different styles and themes
-	responsiveness for all devices

###What are the main goals of leaflet JS? 

-	**Performance: **
Leaflet JS focuses on becoming as light weight as possible while maintaining all map functionality. It does that by optimizing the algorithms and the graphics and even cutting as much unused or dead code as possible from the source code reaching about 39 KB of JS and 4 KB of CSS.
-	**Completeness: **
Even though Leaflet JS seeks to improve efficiency and reduce the size of the code required, it provides all the interactive mapping functionality that most developers would ever require.
-	**Responsiveness and SEO optimization: **
Leaflet shrinks and expands map elements to provide a variety of mobile-friendly displays. To get good readability results from the Google search engine, the library provides lightweight graphs and cutting edge loading time (SEO optimized).
-	**Customizability: **
Leaflet allows third-party themes to be applied to its maps in addition to adding custom stylesheets to all components (such as objects and viewing window).
-	**Accessibility & Availability:  **
Leaflet JS is and will continue to be an open-source project and avalible for the public.
-	**Well documented for users and contributors.**

---

## Requirements

Requirements are split in 3 Parts. Those reflect the different views on Leaflet. 
Starting with User-Requirements we cover the needs for the Users perspective. It is said that User means here the real user
such as those who will see the results of this library. Followed by the Programmer-Requirements, here are all needs a developer would love to have in the project. Divided from this we have the third Category, technical-Requirements. 
Technical-Requirements include mostly Requirements needed by Developers but not in a way they will be affected by it directly. 
Note: Some Requirements belong together from different perspectives but are formulated different from each perspective

### User Requirements
<!-- markdownlint-disable-->
| # of user Requirement | User Requirement |
|-----------------|--------------------|
| U1 | As a User i want to Zoom in/out of the map and Elements should hold their relative Position |
| U2 | As a User i want to use Maps with Leaflet independent from my browser |
| U3 | As a User i want to see no differences betweens Elements from Leaflet in different Browsers |
| U4 | As a User i want to have no extra loading/initialization times (no big computation times) |
| U5 | As a User i want to have responsive design |
| U6 | As a User i want to have responsive controls (touchscreen/mouse differ in the way of use) |
| U7 | As a User i want to have a fast reset to original map-settings |
| U7 | As a User i want to switch between metrical and imperial scale |

<!-- markdownlint-enable-->

### Programmer Requirements
<!-- markdownlint-disable-->
| # of Programmer Requirement | Programmer Requirement |
|-----------------|--------------------|
| P1 | As a Programmer i want to implement different Map-Types such that Leaflet works the same way with different Maps |
| P2 | As a Programmer i want to include Animations with or without  CSS |
| P3 | As a Programmer i want to make Elements dragable/movable |
| P4 | As a Programmer i want to Organize Elements in Layers |
| P5 | As a Programmer i want to Overlap the Map with Images/Videos/SVG |
| P6 | As a Programmer i want to have build in functionality for different geometric objects (Lines, Polygons, Squares) |
| P7 | As a Programmer i want to Control the Opacity, Thickness, Color etc for geometric Objects |
| P8 | As a Programmer i want to merge those geometric objects into bigger ones |
| P9 | As a Programmer i want to define Points with Koordinates in the Map |
| P10 | As a Programmer i want to add EventListeners to Elements and the Map itself |
| P11 | As a Programmer i want to have Mod/Plugin Support for Leaflet Library |
<!-- markdownlint-enable-->

### Technical Requirements
<!-- markdownlint-disable-->
| # of Technical Requirement | Technical Requirement |
|-----------------|--------------------|
| T1 | The System should be lightweight and have only the absolute minimum of code needed for the requirements |
| T2 | The System should support plugins such that additional features are easy to implement and keep the code small |
| T3 | The System should work on any plattform that supports JS (Vanilla JS) |
| T4 | The System should work regardless of Browser |
| T5 | The System should be deployable internal and external (JS-File or loaded from a CDN) |
| T6 | The System should have simple, readable source code |
| T7 | The System should support different Map-Distributors such as Google, OpenStreetMap, Bing etc. |
| T8 | The System should be exportable as a single JS File |
<!-- markdownlint-enable-->

## Stakeholder
<!-- markdownlint-disable-->
Text
<!-- markdownlint-enable-->

## View
<!-- markdownlint-disable-->

The main goal of our work is to create the requirements with the right method, which is flexible enough and open to changes and complies with the standards chosen for software development and maintenance.
Because the process of defining, documenting and maintaining requirements in this prject is missing.
<!-- markdownlint-enable-->

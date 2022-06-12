
# TABLE OF CONTENTS

1. [Introduction](#introduction)
   1. [Functionalities](#functionalities)
   2. [Main goals](#main-goals)
2. [Stakeholders](#stakeholders)
3. [Requirements](#requirements)
   1. [User Requirements](#user-requirements)
   2. [Programmer Requirements](#programmer-requirements)
   3. [System Requirements](#system-requirements)
4. [Outlook](#outlook)
5. [Glossary](#glossary)

## Introduction

Leaflet is a simple, performant, lightweight JavaScript Library to enable simple handling for interactive Maps.  It is used by many large Corporations such as GitHub, Etsy, Facebook, etc.
In Part 1 of our project, we roughly compiled and formulated the requirements of Leaflet.
Since the requirements are not formulated in Leaflet, we have set ourselves the goal of making the requirements understandable as our contribution, so that certain design decisions are more comprehensible and lead to be incorporated into a uniform architecture. 

[comment]: <> (Leaflet is a simple, performant, lightweight JavaScript Library to enable simple handling 
for interactive Maps. This Document defines several Requirements that shall be satisfied by Leaflet. 
Those Requirements are created by Reengineering since Leaflet has no Requirements and Analysis till Version 1.8.0 and only 
provides Documentation about the API for Devs. We aim to improve this by Contributing to the Project so that those Requirements get more clear for every new
Developer so that they easily understand why certain design decisions were made. It also helps to maintain the Code in a better way.
Leaflet sets its target 100% on simplicity and performance. This said we will always keep it in mind when making any decisions about refactoring code.
It is said that Leaflet is used by many large Corporations such as GitHub, Etsy, Facebook, etc. Because it is a widespread project, it is needed to have 
a flawless Documentation of every development step.)

### Functionalities

-	Creating lightweight maps in simple readable code.
-	customizability with different styles and themes
-	responsiveness for all devices

### Main goals

-	**Performance:**
Leaflet JS focuses on becoming as lightweight as possible while maintaining all map functionality. It does that by optimizing the algorithms and the graphics and even cutting as much unused or dead code as possible from the source code reaching about 39 KB of JS and 4 KB of CSS.
-	**Completeness:**
Even though Leaflet JS seeks to improve efficiency and reduce the size of the code required, it provides all the interactive mapping functionality that most developers would ever require.
-	**Responsiveness and SEO optimization:**
Leaflet shrinks and expands map elements to provide a variety of mobile-friendly displays. To get good readability results from the Google search engine, the library provides lightweight graphs and cutting-edge loading time (SEO optimized).
-	**Customizability:**
Leaflet allows third-party themes to be applied to its maps in addition to adding custom stylesheets to all components (such as objects and viewing window).
-	**Accessibility & Availability:**
Leaflet JS is and will continue to be an open-source project and is available for the public.
-	**Well documented for users and contributors.**

## Stakeholders

Leaflet is strongly aimed to satisfy the Developer's needs. Nonetheless, the Library defines two Stakeholders. Those are the Users who will see the Effects of Leaflet and the Developers who will
use Leaflet for their projects. Users will see effects from Leaflet through a Browser or any Project based on JavaScript. Users want Leaflet because it provides all the functions you would need on a map in your browser. Additionally, it is lightweight so a User will enjoy the library without even noticing that extra libraries were loaded.
Developers will use Leaflet in their Projects because it provides an easy Interface to use Maps in projects and is also independent of the runtime since it is written in JavaScript so the developers don't have to care about System-Dependencies. Leaflet is a standalone Library so Leaflet will enhance the development process for developers.


## Requirements

Requirements are split into 3 Parts. Those reflect the different views on Leaflet. 
The first two Parts are based on User Requirements. Users are split into two groups, User and Developer.
Starting with User-Requirements we cover the needs from the User's perspective. It is said that User means here the real user
such as those who will see the results of this library. Followed by the Programmer-Requirements, here are all needs a developer would love to have in the project. Divided from this we have the third Category, technical-Requirements. 
System-Requirements include mostly Requirements needed by Developers but not in a way they will be affected by it directly. 
Note: Some Requirements belong together from different perspectives but are formulated differently from each perspective, they are marked together in the Column Type.

### User Requirements
<!-- markdownlint-disable-->
| # of user Requirement | User Requirement | Type | Tracing |
|-----------------|--------------------|--------------------|--------------------|
| U1 | As a User, I want to Zoom in/out of the map, and Elements should hold their relative Position | Functional  |  |
| U2 | As a User, I want to use Maps with Leaflet independent of my browser | Quality  | T4 & T5 |
| U3 | As a User, I want to see no differences between Elements from Leaflet in different Browsers | Quality  | T5 |
| U4 | As a User, I want to have no extra loading/initialization times (no big computation times) | Performance  | |
| U5 | As a User, I want to have responsive design | Quality | P2 |
| U6 | As a User, I want to have responsive controls (touchscreen/mouse differ in the way of use) | Quality | P2 |
| U7 | As a User, I want to have a fast reset to original map settings | Functional | |
| U7 | As a User, I want to switch between metrical and imperial scale | Functional | |

<!-- markdownlint-enable-->
### Programmer Requirements
<!-- markdownlint-disable-->
| # of Programmer Requirement | Programmer Requirement | Type | Tracing |
|-----------------|--------------------|--------------------|--------------------|
| P1 | As a Programmer, I want to implement different Map-Types such that Leaflet works the same way with different Maps | Functional | |
| P2 | As a Programmer, I want to include Animations with or without CSS | Functional | U5 & U6 |
| P3 | As a Programmer, I want to make Elements draggable/movable | Functional | |
| P4 | As a Programmer, I want to Organize Elements in Layers | Functional | |
| P5 | As a Programmer, I want to Overlap the Map with Images/Videos/SVG | Functional | |
| P6 | As a Programmer, I want to have build-in functionality for different geometric objects (Lines, Polygons, Squares) | Functional | |
| P7 | As a Programmer, I want to Control the Opacity, Thickness, Color, etc for geometric Objects | Functional | |
| P8 | As a Programmer I want to merge those geometric objects into bigger ones | Functional | |
| P9 | As a Programmer I want to define Points with Koordinates in the Map | Functional | |
| P10 | As a Programmer I want to add EventListeners to Elements and the Map itself | Functional | |
| P11 | As a Programmer, I want to have Mod/Plugin Support for Leaflet Library | Functional | T3 |
<!-- markdownlint-enable-->
### System Requirements
<!-- markdownlint-disable-->
| # of Technical Requirement | Technical Requirement | Type | Tracing |
|-----------------|--------------------|--------------------|--------------------|
| T1 | The System should have 0 dependencies | Constraint | T3 & T6 |
| T2 | The System should be lightweight and have only the absolute minimum of code needed for the requirements | Constraint | |
| T3 | The System should support plugins such that additional features are easy to implement and keep the code small | Functional & Quality | P11 & T1 |
| T4 | The System should work on any platform that supports JS (Vanilla JS) | Quality | T5 & U2|
| T5 | The System should work regardless of Browser | Quality | T4 & U2 & U3|
| T6 | The System should be deployable internal and external (JS-File or loaded from a CDN) | Constraint | T1 |
| T7 | The System should have simple, readable source code | Quality | |
| T8 | The System should support different Map-Distributors such as Google, OpenStreetMap, Bing, etc. | Quality | |
| T9 | The System should be exportable as a single JS File | Functional | |
| T10 | The System must support automatic testing for several browsers | Quality | |

<!-- markdownlint-enable-->
## Outlook
<!-- markdownlint-disable-->

Because the process of defining, documenting and maintaining requirements in this project is missing we have the target to contribute to the project this missing piece. Our Contribution should enhance the whole Requirement Process. We want to help new Developers too easily understand designing decisions and also offer experienced developers a place to come back and get their minds straight for the goal of Leaflet. The first Contribution will be that this scoping_document will be translated into an HTML File which can be merged into the leafletjs.com Website in the Docu Part.
Leaflet also has over 300 issues on its GitHub, we plan to support the team with some bug fixes. 

<!-- markdownlint-enable-->
## Glossary
<!-- markdownlint-disable-->
| Term | Meaning | 
|-----------------|--------------------|
| JavaScript | The Programming Language Leaflet uses |
| Stakeholder | Person or Group involved in the usage of Leaflet |
| CDN | Content Delivery Network - deliver Code or Text fast from a Network of Servers |
| Requirement(s) | Wishes and Needs for the project |
| Vanilla JS | JavaScript out-of-the-box without any dependencies |
| Mod / Plugin | Code that improves Leaflet without belonging to the Core of Leaflet |
| Layer | a theme or overlay of the map |
| popup | an information window that opens in the viewing frame of the map |
| marker | a pin or an image that marks geographical locations on the map |
| Tooltip | a window the same as a popup but for the locations |
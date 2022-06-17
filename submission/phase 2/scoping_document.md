
# TABLE OF CONTENTS

1. [Introduction](#introduction)
   1. [Functionalities](#functionalities)
   2. [Main goals](#main-goals)
3. [Constraints](#constraints)
4. [Context & Scope](#context)
5. [Solution Strategy](#solution)
6. [Building Block View](#building)
7. [Runtime View](#runtime)
8. [Deployment View](#deployment)
9. [Crosscutting Concepts](#crosscutting)
10. [Architectural Decisions](#architectural)
11. [Quality Requirements](#quality)
12. [Risks & Technical Dept](#risks)
13. [Glossary](#glossary)

## Introduction

Leaflet is a simple, lightweight JavaScript Library to enable simple handling for interactive Maps.  It is used by many large Corporations such as GitHub, Etsy, Facebook, etc.
In Part 1 of our project, we roughly compiled and formulated the requirements of Leaflet.
Since the requirements are not formulated in Leaflet, we have set ourselves the goal of making the requirements understandable as our contribution, so that certain design decisions are more comprehensible and lead to be incorporated into a uniform architecture. 

### Functionalities

-	Creating lightweight maps in simple readable code.
-	customizable with different styles and themes.
-	responsiveness for all devices.

### Main goals (Quality aspects)

-	**Performance:**
Leaflet Js focuses mainly on performance and displaying the features in most appealing way with as less weight as possible.
	-	**Light weight:** Leaflet JS runs as lightweight as possible while maintaining all map functionality. It does that by optimizing the algorithms and the graphics and even cutting as much unused or dead code as possible from the source code reaching about 39 KB of JS and 4 KB of CSS.
	-	**feature Completeness:**
Even though Leaflet JS seeks to improve efficiency and reduce the size of the code required, it provides all the interactive mapping functionality that most developers would ever require.
-	**Documentation** 
The project is well documented for users and contributors.
-	**Usability:**
Leaflet Js focuses mainly on performance and displaying the features in most appealing way with as less weight as possible.
	-	**Responsiveness:** Leaflet shrinks and expands map elements to provide a variety of mobile-friendly displays. To get good readability results from the Google search engine, the library provides lightweight graphs and cutting-edge loading time (SEO optimized).
	-	**compatibility:**
Leaflet JS have a great ability to work with third party plugins support and have a welcoming community for contributors and maintainers.
	-	**Dependability:**
Leaflet JS can work with different browsers with different JS frameworks.
-	**Modifiability:**
Leaflet maps can be modified in many ways.
	-	**Elements modifiability:**
Even though Leaflet JS seeks to improve efficiency and reduce the size of the code required, it provides all the interactive mapping functionality that most developers would ever require.
	-	**Style modifiability:**
Even though Leaflet JS seeks to improve efficiency and reduce the size of the code required, it provides all the interactive mapping functionality that most developers would ever require.
-	**Reliability:**
Leaflet stays reliable under usage pressure. It does that by:
	-	**Maintainablity:**
Since it is an open source project and has a scalable architecture, it has a high level of adaptation to any new issue in the project.
	-	**Testability:**
Leaflet can be tested automatically from browsers thanks to its modularity and scalable architecture.

Various Quality Aspects are defined in the following Quality - Tree. The First Layer from the tree define the bigger goals for leaflet and the leafs of the tree are a bit more precise. The leafs get even more precise in the Requirements. 

![Figure 1: Quality - Tree](./../phase1/qualityAspekts/qualityTree_v2.png)

> NOTE: Mapping the leafs of the quality-tree to the requirements is directly mentioned in the requirement-tables.

## Constraints


## Context & Scope


## Solution Strategy


## Building Block View


## Runtime View


## Deployment View


## Crosscutting Concepts


## Architectural Decisions


## Quality Requirements


## Risks & Technical Dept


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
| Dependence | Libraries or Plugins from third-party providers |
| End user | A person who interacts with the product with the intention of only using the product for his needs |
| Developer | A person who interacts with the product with the intention of using the product for his needs and contributing to the development of the product |

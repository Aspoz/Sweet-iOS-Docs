---
layout: page
title: "2. Controllers"
category: front
date: 2015-01-12 16:50:00
---


The controllers which are provided in the 'Controllers' folder in the project, are almost all the same. Each controller uses the same functions, or a few. The `viewDidLoad` can be found in every controller. This function provides 'configurations' for a few which should be loaded at the moment of loading the view. 

Other re-used functions are the functions which are capable of filling in tables, prepareForSegue information and functions which start API calls.

The tables which get filled, get their data from the API calls and are 'pushed' into models to fill the tables. Segue information, sets data, if it's needed in another views.

Rest functions are specific for that view and will explain themselves, an example is the filtercontrol.

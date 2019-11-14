# Introduction to Decoupled Architectures

## Overview
* Your architecture now supports hundreds of thousands of users, but if one part fails, the whole app fails. You need to remove dependencies.

## What does Tightly Coupled mean?
* Components are strongly tied to each other.
* Traditional infrastructures revolve around chains of tightly integrated servers, each with a specific purpose. 
    * When one of those components/layers goes down... 
        * The disruption to the system can ultimately be fatal 
        * Scaling is impeded
        * To fix: add or remove servers at one layer, every server on every connecting layer has to be connected appropriately


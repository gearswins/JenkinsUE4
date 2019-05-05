# Jenkins UE4
Documentation and Jenkins pipeline for Epic's Unreal Engine 4

## Important Note
This project is under development, no guaranty given.
Do not use on project without backup / source control !

## Introduction

This project is about setting up a Jenkins server and pipelines for UE4 project(s) on a windows machine.
Only tested on Windows 10 with administrator rights.
Using perforce 2018.2 as source control.

A big part of this setup is only required for teams that will make modifications to UE4 source code.

Part of this setup is done by downloading the engine directly from Epic's GitHub.
Note that a work in progress pipeline allow to automaticly download the engine from Epic's github or Perforce and upload it to another Perforce(Replicate.java)

## Some links

Jenkins
https://jenkins.io/

Unreal
https://www.unrealengine.com

## Documentations

[Engine and perforce setup](Documentation/SETUP.md)

[Additional useful setup](Documentation/ADD_SETUP.md)

[Perforce tips](Documentation/P4_TIPS.md)

## Jenkins pipeline

This is the core of the project: a series of Jenkins groovy script that allow you to automate task using UE4 like compilation, create package, Fill the Shared Derived data cache, etc.

[jenkins pipeline](Pipelines/.)

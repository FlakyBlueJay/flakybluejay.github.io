---
title: Tag Hierarchy Manager
tags:
  - CSharp
  - Avalonia
  - DotNET
---
![](taghierarchymanager.png)

This is an application I wrote to manage tag hierarchy templates, a form of text file specific to MusicBee aimed at filtering files hierarchically in a music library based on the audio files' tag contents. With how complex RYM’s tree is, it was worth it for me to write an app for it so it was easy for me to manage. Initially it was written in Python using PyQt, and is still a Qt5 app because at the time, I couldn’t be arsed to port it to Qt6, and the code was a bit of a mess.

I decided to port it to .NET/C# instead since I felt C# was a better language for me, starting with Terminal.Gui, and then eventually, Avalonia. This was what made the MVVM (Model-View-ViewModel) architecture for software click for me - and frankly, if you’re using Avalonia you need to learn it if your app gets to a certain size, since it enforces it quite strictly. I still sometimes get the View and ViewModel a bit blurred with the code-behind, but even then it’s made the code a lot more manageable.

[Available on GitHub](https://github.com/FlakyBlueJay/TagHierarchyManager)
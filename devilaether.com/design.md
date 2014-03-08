# Notes on devilaether.com Design

## Contents
1. Overview
2. Features
3. Ideas

## Overview
The idea is to design a note-taking system that enables quick web publishing. 

## Features
The following is a list of desired features

1. Interfaces: There should be a few quick and easy ways to create and edit notes - from text editors, a web interface, to mobile apps
2. Writing Formats: The system should support notes in plain text, Markdown and HTML. 
3. Version Control: The system must have a version control backend. Treat notes as code. 
4. Storage: All notes should be kept as plain text files.
5. Incremental Feature Development: I have ** other ** projects. I need to take notes ** now **.

## Ideas
### Scenario 1: A Workflow with a Text Editor
1. I am coding and using a text editor
2. I have an idea I need to research later, but must not forget. I should take a note.
3. I open a new file in the text editor and write down my idea. Brilliant.
4. I save the file. It would be nice to share this with another developer for comments - I should publish it.
5. My sharing options:
* Paste the note in a gist and IM the dev the URL, like any code snippit.
* Commit the note to a github repo and IM the others about new notes
* Run the note through Markdown and upload the file to a web server.
* Commit note to github, refresh working copy on web server, run markdown on tree, publish.
6. Thing is, I just want to write the note and it gets magically published.
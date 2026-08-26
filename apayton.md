# Final Proposal

## Overview:
Develop a web extension created with the intention of detecting AI generated content and differentiating it between real content. It would mainly target AI images as they contain meta-data and artifacts of AI creation that would be able to be targeted automatically as they appear. A user could configure the extension to install and uninstall with ease, stop and start the process, and alter the confidence score required to flag something as AI generated. It would be as lightweight and unobtrusive as possible.

## Why:
The problems that this solves depends on what the user wants from it. A user could be using this extension in order to be more aware of the media they consume, differentiate real and false information, or tell which artists or creators use AI. From a larger scope, it solves an issue of the trade-off between checking the authenticity of an image and the time, skill, and knowledge in order to do so.

## What:
The major feature that I would want is for it to be able to run automatically in the background of a web browser without massive bloat. For detection of AI images there are a few methods that could be applied such as signature and heuristic based detection. A database would store images of AI content and be able to compare new images to that of the saved images and compare if they are the same or similar. Next, a method of [mathematically analyzing an image](https://arxiv.org/html/2502.15176v2) and grabbing meta-data could be applied on top of that. 

## How:
Most of the project would be written in JavaScript as it would be a web extension. There would be other tools required for the framework that web extensions use such as ‘manifest.js’, ‘content.js’, and ‘background.js’. Likely a form of database would be required using a type of SQL server. Lastly would be the methods required to be able to analyze images for AI artifacts and meta-data, likely using Python.

## Who
The intended user of this software would be a broad scope of individuals who have concerns of AI images on the web. It would be targeted towards those who lack the technical knowledge to be able to detect images for themselves, or are too lazy in order to do so for any image that they see, automating the process.

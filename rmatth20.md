# PaperPal - A paper-to-pdf notetaking tool

## Introduction

This project aims to improve notetaking for students by scanning their notes into our software, which will allow them to clean them up through various methods. The project will use Machine Learning models and smart OCR classification to transform notes into a more digestible format.

## What is on offer?

We aim to implement many useful features that will transform regular notes into something useful. Poor handwriting? Turn it into a printed font. Messy diagrams? Rearrange and replace them in the software. We could even add in LLM integration that suggests review topics or highlights key parts of the notes.

## Format

We will utilize a Python Backend building the basic OCR off of TrOCR or PaddleOCR to overcome the inital text recognition step. Then, we will combine a traditional interpreter with other Machine Learning models to improve text classification and formatting power. We aim to keep everything hosted locally to the user to allow offline, private utilization. This would also allow us to keep the software free, which is a major leg up against competitors.

## Goals

- Implement a working text recognition base, and develop a classification software on top of it that allows high fidelity transfer to a digital format.
- Implement an editor space that allows users to format the document the way that they prefer and fix any mistakes that the OCR makes.
- Implement presets that will auto-format notes.
- Keep everything local and free, if users prefer, but also allow for expansion into the GenAI space.

## Audience

This software will be targted at high school and college students. These are the main people taking notes for classes, so that is the main use case for a notes app. This could eventually be expanded to include notes for meetings, creating to-do lists, and including voice-notes or summarizing lectures as well. This makes notes easier to come back to, more concise, and more easily shareable, and also relieves the difficulty of taking notes neatly on the first pass. Instead, our software allows one to take notes quickly or messily at first, and then clean them up in a less demanding environment.


# Project Proposal

## Project Summary

This project is a mobile app that helps blind people navigate grocery shopping using their phone's camera. Users can point their camera at produce or any barcoded goods to hear an identification read aloud. Unlike general-purpose identification apps, this project is built specifically around grocery products, and it improves over time through user feedback rather than relying on a fixed dataset. It also gives users a way to connect with and help others who deal with the same challenges.

## What Problem It Solves

Produce and bulk items rarely have accessible labeling, and existing identification tools require a live human to be available on the other end of a call, which isn't always practical. This project combines on-device visual identification with a community-driven correction system, so that the app gets more accurate over time instead of staying static.

## Major Features

* Live camera scanning that identifies produce and packaged items and reads results aloud
* Barcode scanning for packaged goods, pulling verified product and ingredient info
* Voice-based correction/tagging so users can fix a wrong identification, improving accuracy for all app users
* Voice-first interface designed to work with screen readers
* Adjustable verbosity/speed settings for audio feedback

## Technologies/Requirements

* **Frontend:** React Native or Flutter
* **Backend:** Node.js/Express or Python/FastAPI to manage the community tagging and correction data
* **Database:** Postgres or Firebase to store product corrections, user preferences, and cached identification results
* **Vision/Recognition:** Google Cloud Vision API or ML Kit for image-based produce identification
* **Barcode Data:** Open Food Facts API or a similar product database for packaged goods
* **Text-to-Speech:** native platform TTS (iOS AVSpeechSynthesizer / Android TextToSpeech) for audio feedback
* **Hosting:** Vercel/Render for backend services, with app builds distributed via TestFlight/internal Android testing

## Intended Users

The intended users are blind and low-vision individuals who want more independence when grocery shopping, and want to do something for their community of other low-vision people.


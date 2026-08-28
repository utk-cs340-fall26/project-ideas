# Project Proposal: Tabletop

## The Idea

Tabletop is a mobile app that makes your phone into a card table. You bring your phone near a friends and a game lobby instantly opens on both screens. You're betting fake chips that don't hurt your pocket but can still be used as currency in the app. You can buy card backs, tables, animations, chip skins, etc.. All to flex on your friend across the table.

## The Problem
Mobile games are lonely. Even if you are playing online on them, you're more than likely playing with strangers in a different country. Meanwhile, people spend time together in real-life, just scrolling on their phones. Whether you're waiting for your food, sitting on a train, or killing twenty minutes before class- Tabletop gives you a way to enjoy your friends' company on the go.

Physical card games solve this, but you can't expect every situation to be right to setup a deck. Tabletop is already in your pocket, and unlike a real deck you can rock cool cosmetics.

## Major Features

* **Proximity games**: Once you open the app and are close to your friend, you can instantly hop in a game. QR codes and 4-character room code would work as fallbacks.
* **Heads Up Blackjack**: This is a super easy game for everyone to understand, is easy to build, and is super fun. Perfect for our MVP.
* **Cosmetics**: Purchase all kinds of cosmetics with your hard earned chips.
* **Daily chip refill**: Nobody is ever fully locked out. Daily chip refills with other ways to earn extra.
* **Cosmetic storefront**: Item Shop with rotating items that you can buy.
* **Guest mode**: You can play immediately, even without an account. Frictionless.

## Tech

This will be built in Expo which is a React Native wrapper that improves the developer experience substantially. The authentication will be using Better Auth.

We should have a central backend in TypeScript using Fastify. It will use Postgres for accounts/inventory and Redis for live game state. Everything handled server side to prevent cheating. 

## Who It's For

It's for adults between 18-30 who enjoy playing games on their phone and spend time in groups. The app must be rated 18+ due to simulated gambling guidelines on the App Store.

They would want this because it's a way to give a meaning to playing meaningless games with your friends. It's a number that goes up when you win and goes down when you lose. It's just another thing to brag about.

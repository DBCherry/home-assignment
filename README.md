# Full-Stack Home Assignment: Tic-Tac-Toe Game

## Project Description

Develop a full-stack application for a tic-tac-toe game where human users can play against an AI bot.

## Required Stacks

- **Database**: MongoDB
- **Backend**: TypeScript + Nest.js
- **Frontend**: TypeScript + Next.js

## Preferred Libraries

- **Backend**
  - Mongoose.js
- **Frontend**
  - MUI
  - Tailwind CSS
  - React Query + Axios

## Required Features

### 1. Gameplay

- Users should be able to play a game of tic-tac-toe against an AI bot at a variety of levels of difficulties.
- Users are able to switch the difficulty during the gameplay.
- Users always start the game.

### 2. Game Statistics

- After each game, the system should update the game statistics for the player.
- The statistics should include the number of games won, lost, and drawn by the player.

### 3. Backend API Endpoints

- Gameplay API endpoint whose

  - request method is POST
  - request header includes
    - user email;
    - difficulty; "easy" | "medium" | "hard"
  - request body includes the user action which are;
    - row; number from 0 to 2
    - col; number from 0 to 2
  - response body includes the game status and the AI bot response which are;
    - status; "idle" | "won" | "lost" | "drawn"
    - row; number from 0 to 2
    - col; number from 0 to 2

- Statistics API endpoint whose

  - request method is GET
  - request header includes user email
  - response body includes game statistics;
    - won; number of games won
    - lost; number of games lost
    - drawn; number of games drawn
    - total; total number of games played

## UI Mockup

- UI should include
  - Input box for user's email
  - Select box for difficulty level; Easy / Normal / Difficult
  - Statistics card
  - Game playboard

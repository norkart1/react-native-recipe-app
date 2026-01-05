# React Native Recipe App

## Overview
A full-stack recipe application with a React Native mobile frontend (Expo) and Express.js backend API.

## Project Structure
- `/backend` - Express.js API server with Drizzle ORM and PostgreSQL
- `/mobile` - React Native/Expo mobile application

## Backend API
- **Port**: 5000
- **Database**: PostgreSQL with Drizzle ORM
- **Endpoints**:
  - `GET /api/health` - Health check
  - `POST /api/favorites` - Add favorite recipe
  - `GET /api/favorites/:userId` - Get user's favorites
  - `DELETE /api/favorites/:userId/:recipeId` - Remove favorite

## Technology Stack
- Backend: Express.js, Drizzle ORM, PostgreSQL
- Mobile: React Native, Expo, Clerk (authentication)

## Running the Project
- The backend API runs on port 5000 via the "Backend API" workflow
- The mobile app requires Expo Go on a physical device or emulator

## Database Schema
- `favorites` table: stores user's favorite recipes with id, userId, recipeId, title, image, cookTime, servings, createdAt

## Environment Variables
- `DATABASE_URL` - PostgreSQL connection string (auto-configured by Replit)
- `EXPO_PUBLIC_CLERK_PUBLISHABLE_KEY` - Required for mobile app authentication (user must provide)

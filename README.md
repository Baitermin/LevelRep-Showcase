<div align="center">

# 🏋️ LevelRep

### Every rep levels you up.

A cross-platform fitness app focused on **personalized training, progression and motivation**.

![Repository](https://img.shields.io/badge/Source-Private-6e7681?style=flat-square&logo=github)
![Status](https://img.shields.io/badge/Status-Active_Development-f59e0b?style=flat-square)
![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Expo](https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white)

</div>

---

## Overview

LevelRep is an iOS and Android fitness app built around a simple long-term loop:

> **Plan → Train → Measure → Adapt → Progress → Repeat**

The goal is to combine traditional workout tracking with adaptive training, progressive overload and gamification without turning the app into a generic fitness dashboard.

The production source repository is private while the application is under active development. This repository is the public showcase for the project, its architecture, current progress and roadmap.

---

## Current Status

**Phase 1 — Foundation is complete.** The current app has been validated end-to-end against a live Supabase backend.

### Implemented today

- Email/password authentication
- Google OAuth through Supabase Auth
- Persistent authenticated sessions
- First-login username setup
- One-question-per-screen onboarding flow
- Training profile and preference editing
- Equipment selection
- Private avatar uploads
- Dark reusable design system
- Secure Postgres schema with Row Level Security
- Client + database validation
- CI checks for linting, TypeScript and tests
- Android development builds through Expo/EAS

The main Home, Train, Calendar and Social areas are currently foundation placeholders while the workout engine and later product phases are built.

---

## Product Roadmap

| Phase | Scope | Status |
| --- | --- | --- |
| 1 | App foundation, auth, onboarding, profile, design system & backend | ✅ Complete |
| 2 | Exercise library, workout logging, history & personal records | ⬜ Planned |
| 3 | Adaptive training engine & AI provider layer | ⬜ Planned |
| 4 | XP, levels, achievements & streaks | ⬜ Planned |
| 5 | Friends, challenges & leaderboards | ⬜ Planned |
| 6 | Notifications, offline support & release preparation | ⬜ Planned |

---

## Planned Experience

### 🧠 Adaptive Training

Training plans will adapt from structured user data and recent performance rather than treating the AI model as the database or rules engine.

Planned inputs include:

- Goals and training experience
- Available training days
- Session duration
- Available equipment
- Recent performance and progression
- Training volume and consistency
- Exercise preferences and constraints

### 📈 Progression

The workout core is planned around measurable progression:

- Workout history
- Sets, reps and weight tracking
- Personal records
- Progressive overload
- Training analytics
- Recent-performance summaries

### 🎮 Gamification

Motivation is a core product feature rather than a cosmetic layer.

Planned systems include:

- XP and levels
- Badges and achievements
- Training streaks
- Challenges with friends
- Leaderboards

---

## Architecture

### Mobile

- **Expo SDK 57**
- **React Native**
- **TypeScript**
- **Expo Router** for file-based navigation
- **React Native Reanimated** and native interaction libraries

### Backend

- **Supabase Auth**
- **PostgreSQL**
- **Row Level Security**
- Version-controlled SQL migrations
- Private storage for user avatars

### State & Data

- **Zustand** for local/ephemeral UI state
- **TanStack React Query** for backend-backed server state
- **AsyncStorage** for persisted local onboarding state
- **Zod** for client-side schemas and validation

### Quality

- **Jest**
- **Testing Library for React Native**
- **ESLint**
- **Prettier**
- Strict TypeScript checks
- Automated CI on pushes and pull requests

---

## Privacy & Source Code

The main LevelRep repository is intentionally private while the product is being designed and developed.

This showcase contains **no credentials, private backend configuration or proprietary source code**. It exists to document the product, technology choices and development progress publicly.

---

<div align="center">

**Built by [Baitermin](https://github.com/Baitermin)**

🚧 LevelRep is actively being developed.

</div>

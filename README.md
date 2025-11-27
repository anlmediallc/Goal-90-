# Goal 90 - Footwork Training Application

**Phase 1: Foundation & Core Features**

A mobile-first football (soccer) footwork training web application that delivers structured video lessons with gamification features to motivate users.

## Overview

Goal 90 is a sports training platform focused on teaching football footwork skills through organized video lessons. The application uses points, streaks, and achievements to keep users engaged and motivated in their training journey.

## Features

### Authentication
- Password-based login system
- Session management for secure access

### Training Modules
- 5 structured training modules covering different skill areas:
  - Ball Control Fundamentals
  - Speed & Agility
  - Dribbling Techniques
  - First Touch Mastery
  - Match Situations

### Lesson System
- Video-based lessons within each module
- Progress tracking for completed lessons
- Points awarded for lesson completion

### Gamification
- Points system to track overall progress
- Daily streak tracking to encourage consistency
- Achievement badges for reaching milestones
- User profile displaying stats and accomplishments

### User Interface
- Mobile-first responsive design
- Dark theme optimized for video viewing
- Energetic green and orange color scheme
- Thumb-friendly bottom navigation
- Smooth animations and transitions

## Tech Stack

### Frontend
- React 18 with TypeScript
- Vite (build tool)
- Wouter (routing)
- TanStack React Query (server state management)
- Shadcn/ui (UI components)
- Tailwind CSS (styling)

### Backend
- Express.js (REST API server)
- Session-based authentication
- PostgreSQL database
- Drizzle ORM

### Database Schema
- Users (authentication and stats)
- Modules (training content organization)
- Lessons (video content)
- User Progress (completion tracking)
- Achievements (gamification)
- User Achievements (unlocked badges)

## Getting Started

### Prerequisites
- Node.js installed
- PostgreSQL database

### Installation

1. Install dependencies:
```bash
npm install
```

2. Set up the database:
```bash
npm run db:push
```

3. Seed initial data:
```bash
tsx server/seed.ts
```

4. Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:5000`

### Default Login
- Password: `goal90`

## Project Structure

```
├── client/              # Frontend React application
│   ├── src/
│   │   ├── components/  # Reusable UI components
│   │   ├── pages/       # Page components (Login, Home, Profile, etc.)
│   │   ├── lib/         # Utilities and configuration
│   │   └── hooks/       # Custom React hooks
├── server/              # Backend Express server
│   ├── index.ts         # Server entry point
│   ├── routes.ts        # API route definitions
│   ├── storage.ts       # Database access layer
│   ├── seed.ts          # Database seeding script
│   └── vite.ts          # Vite integration
├── shared/              # Shared code between client and server
│   └── schema.ts        # Database schema and types
└── db/                  # Database configuration
```

## Development Roadmap

### Phase 1: Foundation (Current)
- ✅ User authentication
- ✅ Module and lesson structure
- ✅ Video player
- ✅ Progress tracking
- ✅ Points and streaks
- ✅ Achievement system
- ✅ User profile

### Future Phases
- Real video content integration
- Social features (sharing progress)
- Advanced analytics
- Mobile app version
- Personalized training plans

## Design Philosophy

The application draws inspiration from successful fitness apps like Nike Training Club and Strava, emphasizing:
- Clear visual hierarchy
- Motivational design elements
- Easy-to-track progress
- Consistent and energetic branding
- Accessibility and mobile-first approach

## License

Private project - All rights reserved

## Contact

For questions or feedback about this project, please reach out through the project repository.

---

**Phase 1 - Initial Implementation**
Built with React, TypeScript, Express, and PostgreSQL

# 🧠 AI Mental Health Companion

An open-source, AI-powered mental health support platform that provides 24/7 emotional support, mood tracking, and crisis intervention capabilities.

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![TypeScript](https://img.shields.io/badge/TypeScript-007acc?logo=typescript&logoColor=white)](https://typescriptlang.org)
[![Next.js](https://img.shields.io/badge/Next.js-000000?logo=nextdotjs&logoColor=white)](https://nextjs.org)
[![Prisma](https://img.shields.io/badge/Prisma-2D3748?logo=prisma&logoColor=white)](https://prisma.io)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css&logoColor=white)](https://tailwindcss.com)

## 🌟 Features

### Core Functionality
- **🤖 AI Chat Support**: GPT-4 powered empathetic conversations
- **📊 Mood Tracking**: Daily mood logging with analytics
- **🎯 Goal Setting**: Personal mental health goal management
- **⚠️ Crisis Detection**: Automatic risk assessment and intervention
- **📱 Progressive Web App**: Works offline, installable
- **🔒 Privacy First**: Anonymous usage options, secure data handling

### Advanced Features
- **📈 Insights & Analytics**: AI-generated personal insights
- **🚨 Emergency Contacts**: Crisis intervention system
- **🌍 Multi-language Support**: Internationalization ready
- **🎨 Accessibility**: WCAG 2.1 AA compliant
- **🔄 Real-time Sync**: Cross-device synchronization
- **📝 Journal Integration**: Mood journaling with AI feedback

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ 
- PostgreSQL database
- OpenAI API key
- Clerk account (for authentication)

### Installation

```bash
# Clone the repository
git clone https://github.com/ArnaudBand/mental-health-companion.git
cd mental-health-companion

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env.local
# Edit .env.local with your API keys and database URL

# Set up the database
npx prisma db push
npx prisma db seed

# Start development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to see the application.

## 🏗️ Tech Stack

### Frontend
- **Next.js 15** - React framework with App Router
- **TypeScript** - Type-safe JavaScript
- **Tailwind CSS** - Utility-first CSS framework
- **shadcn/ui** - Beautiful, accessible components
- **Framer Motion** - Smooth animations
- **React Query** - Server state management

### Backend
- **Next.js API Routes** - Serverless API endpoints
- **Prisma** - Type-safe database ORM
- **PostgreSQL** - Relational database
- **OpenAI API** - AI conversation engine

### DevOps & Quality
- **Docker** - Containerization
- **Jest** - Unit testing
- **Playwright** - E2E testing
- **ESLint + Prettier** - Code formatting
- **Husky** - Git hooks
- **GitHub Actions** - CI/CD pipeline

## 📁 Project Structure

```
src/
├── app/                    # Next.js App Router
│   ├── (auth)/            # Authentication pages
│   ├── dashboard/         # Protected dashboard pages
│   └── api/               # API endpoints
├── components/            # Reusable components
│   ├── ui/               # shadcn/ui components
│   ├── auth/             # Authentication components
│   ├── chat/             # Chat interface components
│   └── mood/             # Mood tracking components
├── lib/                   # Utility functions
│   ├── db.ts             # Database connection
│   ├── openai.ts         # AI integration
│   ├── utils.ts          # General utilities
│   └── validations.ts    # Zod schemas
├── hooks/                 # Custom React hooks
├── stores/                # Zustand state management
├── types/                 # TypeScript definitions
└── styles/                # Additional styles
```

## 🔧 Configuration

### Environment Variables

```bash
# Database
DATABASE_URL="postgresql://username:password@localhost:5432/mental_health_db"

# OpenAI
OPENAI_API_KEY=your_openai_api_key

# App Settings
NEXT_PUBLIC_APP_URL=http://localhost:3000
NEXTAUTH_SECRET=your_nextauth_secret
```

### Database Schema

The application uses Prisma with PostgreSQL. Key models include:

- **User**: User profiles and preferences
- **Mood**: Daily mood tracking entries
- **ChatSession**: AI conversation sessions
- **Message**: Individual chat messages
- **Goal**: User-defined mental health goals
- **Insight**: AI-generated recommendations
- **Notification**: System notifications

## 🤖 AI Integration

### OpenAI Configuration
The application uses GPT-4 for:
- Empathetic chat responses
- Mood analysis and sentiment detection
- Crisis risk assessment
- Personalized insights generation

### Safety Features
- Crisis keyword detection
- Risk level assessment
- Emergency contact integration
- Professional help recommendations

## 🧪 Testing

```bash
# Run unit tests
npm test

# Run E2E tests
npm run test:e2e

# Run with coverage
npm run test:ci
```

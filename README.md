# SensAI

SensAI is an AI-powered platform for generating resumes, cover letters, and preparing for interviews. Built with Next.js, Tailwind CSS, Prisma, and Clerk for authentication.

## Features
- AI-generated cover letters and resumes
- Interactive interview preparation and mock interviews
- User onboarding and dashboard
- Secure authentication with Clerk
- Modern UI with Tailwind CSS

## Getting Started

### Prerequisites
- Node.js (v18+ recommended)
- npm or yarn
- A PostgreSQL database (or compatible with Prisma)
- Clerk account for authentication
- Gemini API key for AI features

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/sensai.git
   cd "SensAI Original"
   ```

2. **Install dependencies:**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Set up environment variables:**

   Create a `.env` file in the root directory with the following variables:

   ```
   DATABASE_URL=your_database_url

   NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
   CLERK_SECRET_KEY=your_clerk_secret_key

   NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
   NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
   NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
   NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding

   GEMINI_API_KEY=your_gemini_api_key
   ```

4. **Set up the database:**
   ```bash
   npx prisma migrate deploy
   ```

5. **Run the development server:**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

   Open [http://localhost:3000](http://localhost:3000) in your browser.

## Project Structure

- `app/` - Next.js app directory (routes, layouts, pages)
- `components/` - Reusable UI components
- `actions/` - Server actions for cover letter, resume, interview, user
- `lib/` - Helper functions, Prisma client, utilities
- `prisma/` - Prisma schema and migrations
- `public/` - Static assets

## Scripts

- `dev` - Start the development server
- `build` - Build the application
- `start` - Start the production server
- `prisma` - Prisma CLI for database management

## Note
All features were built and tested locally before pushing the final version. This commit reflects the complete and working project submitted for evaluation.
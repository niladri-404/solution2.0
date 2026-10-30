# APAAR-Connect AI — SOLUTION 2.0
SIH problem statement: SIH26263

An original Next.js website starter for the proposed AICTE student data management and verification platform.

## Included in this build
- Responsive admin-style portal and navigation
- Overview dashboard and enrolment snapshot
- Student records table and add-student workflow
- CSV import and export
- Local duplicate APAAR-like ID and format checks
- Institution directory
- Local demo verification portal
- Programme analytics and audit activity view
- Role-perspective selector
- Vercel-ready Next.js project structure

## Important limitations
This is a functional front-end demonstration with browser-session state and synthetic sample records. It does **not** connect to the official APAAR registry, AICTE systems, DigiLocker or NAD. The APAAR-like ID rule is only a format check, not identity validation. No real student personal data should be entered. Do not represent simulated verification as official verification.

For a production SIH submission, configure a secure backend, persistent database, server-side role permissions, institution onboarding, audit retention, privacy/consent controls, and authorized official API access.

## Run locally (Windows)
1. Install Node.js LTS (https://nodejs.org/).
2. Extract this ZIP.
3. Open the extracted folder in VS Code.
4. Open Terminal → New Terminal.
5. Run:
   ```bash
   npm install
   npm run dev
   ```
6. Open http://localhost:3000

## GitHub
Create a new empty repository in your own GitHub account, then run in this folder:
```bash
git init
git add .
git commit -m "Initial APAAR-Connect AI website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```
Replace the remote URL with your own repository URL.

## Vercel
1. Sign in to Vercel using your GitHub account.
2. Import your new repository.
3. Framework preset: Next.js (normally detected automatically).
4. Deploy. No environment variables are required for this demo.
5. Vercel will provide your own deployment URL.

## Supabase (next backend integration stage)
An `.env.example` file is included. Once a Supabase project and database schema are configured, copy the URL and anon key into Vercel environment variables. Do not put service-role keys in browser code.

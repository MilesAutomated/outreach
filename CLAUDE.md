# CLAUDE.md

## Memory
Long-term memory lives in the private `MilesAutomated/claude-brain` Obsidian vault. If it's attached to the session, follow its `CLAUDE.md`: read `Home.md` and `Projects/Outreach.md` first, and log the session there when done.

## Project
Visitor/outreach web app, originally generated with Bolt (see `.bolt/prompt` for design preferences).

- Vite + React 18 + TypeScript + Tailwind, icons from `lucide-react`
- Supabase (`src/lib/supabase.ts`, migrations in `supabase/migrations/`, main table `visitors`)
- Vapi voice (`@vapi-ai/web`), phone input via `react-phone-number-input` / `libphonenumber-js`
- Deployed on Netlify (`netlify.toml`, `public/_redirects`)

## Commands
- `npm run dev`: local dev server
- `npm run build`: production build
- `npm run lint`: ESLint

## Notes
- `.env` (Supabase URL + anon key) is committed and this repo is public. Don't add any other secrets to it.

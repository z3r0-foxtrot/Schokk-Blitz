# Schokk Blitz Wiki

A modular Next.js wiki starter for the Schokk Blitz Roblox game. The project is designed to be maintained in GitHub and deployed through Vercel.

## Current scope

The first version contains the homepage and reusable layout components only. Directory destinations are placeholders for future modules.

## Stack

- Next.js App Router
- React + TypeScript
- Lucide icons
- CSS custom properties and modular component structure
- Vercel deployment from GitHub

## Run locally

Requires Node.js 20.9 or newer.

```bash
npm install
npm run dev
```

Open http://localhost:3000.

## Deploy through GitHub and Vercel

1. Create a new GitHub repository, for example `schokk-blitz-wiki`.
2. Extract this project and upload its files to the repository root.
3. Commit the files to the `main` branch.
4. In Vercel, choose **Add New → Project**, import the GitHub repository, and deploy.
5. Vercel should detect Next.js automatically. No environment variables are required for this initial homepage.

Every push to the connected production branch will trigger a new deployment.

## Modular structure

```text
app/
  globals.css       Global design tokens and responsive styling
  layout.tsx        Root layout, fonts and metadata
  page.tsx          Homepage route
components/
  layout/
    site-shell.tsx  Shared application frame
    sidebar.tsx     Main navigation
    topbar.tsx      Breadcrumbs and utility controls
  home/
    home-page.tsx   Homepage sections and directory data
```

## Extending the wiki

Recommended next modules:

- `app/towers/` — tower directory and article pages
- `app/enemies/` — enemy directory and article pages
- `app/maps/` — map directory and map details
- `app/equipment/` — equipment database
- `app/guides/` — guides and tutorials
- `app/updates/` — patch notes and change history
- `components/wiki/` — reusable article layouts, infoboxes, tables and content blocks
- `lib/` — content loading, data types, search and permission utilities

## Important notes

- This initial version is a visual homepage prototype, not yet a complete wiki CMS.
- Search, authentication, editing, article storage and role-based permissions are not implemented yet.
- The current directory links are intentionally placeholders.
- The staff-maintained label is branding text; it does not yet enforce access control.
- Replace the placeholder metadata and any future sample content with verified Schokk Blitz information.

# TripTales

TripTales is a responsive travel planner for organizing trips, day-by-day activities, travel budgets, and destination inspiration. Trip data is stored in the browser with LocalStorage.

## Requirements

- Node.js 18 or newer
- npm

## Run locally

```bash
npm install
npm run dev
```

Open the local URL printed by Vite. Create and edit trips, activities, and expenses from the app; changes persist in the current browser.

In Windows PowerShell, if script execution blocks `npm.ps1`, use the Windows command shim:

```powershell
npm.cmd install
npm.cmd run dev
```

## Production build

```bash
npm run build
npm run preview
```

The production files are generated in `dist`.

In Windows PowerShell, use `npm.cmd run build` and `npm.cmd run preview` if `npm` is blocked by the execution policy.

## Deploy to Vercel

1. Import this project in Vercel or run `vercel` from the project directory.
2. Set the build command to `npm run build`.
3. Set the output directory to `dist`.
4. Deploy. No environment variables are required.

## Deploy to Netlify

1. Import this project in Netlify or run `netlify deploy`.
2. Set the build command to `npm run build`.
3. Set the publish directory to `dist`.
4. Deploy. No environment variables are required.

## Notes

- The first visit is populated with editable sample trips.
- Trip records stay on the device and browser where they were created; sharing uses the native share sheet when available, otherwise it copies a trip summary.
- Destination photos are served from Unsplash and require an internet connection.


# Failed Deployment Context

## Deployment Info
- **Deployment ID:** dpl_FRUjP2JTVWdhir8sMNSGvSo25ztq
- **Project:** devbox-todo
- **Team:** vercel-labs
- **Status:** ERROR
- **Error Code:** module_not_found
- **Error Message:** Command "npm run build" exited with 1
- **Error Step:** buildStep
- **Git:** vercel-eddie/devbox-todo@broken2

## Root Cause

`src/app/layout.tsx` imported `formatTitle` from `../utils/format`, but the file `src/utils/format.ts` did not exist.

## Fix

Created `src/utils/format.ts` with the `formatTitle` export.

## Build Logs
```
✓ Compiled successfully in 4.3s
✓ Generating static pages (6/6)
```

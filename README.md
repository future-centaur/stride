# Stride

Stride is a local-first operational task manager built around the loop:

**Define → Execute → Experiment → Observe → Promote → Evolve**

## Current status

This repository is the production source snapshot transferred from the Stride AppDeploy project.

## Development

```bash
npm install
npm run dev
```

Build for production with:

```bash
npm run build
```

## Architecture

- React + TypeScript + Vite
- Tailwind CSS
- Local-first persistence via `localStorage`
- Plan → PlanVersion → Task → TaskStep execution model
- Recurring execution uses a bounded 14-day rolling horizon

## Notes

The application currently stores workspace data locally in the browser. Moving the source code to GitHub does not migrate existing browser-local data between environments or devices.

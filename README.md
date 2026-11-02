# Flipper Web Simulator

A browser-based simulation of the Flipper Zero experience, built with React, Vite, and a lightweight Express server. The app presents a dark, cyber-inspired dashboard that mirrors common Flipper workflows across radio, NFC, BadUSB, GPIO, infrared, iButton, BLE, and file-system modules.

This project is designed for experimentation, demos, and educational exploration without requiring a physical Flipper device.

## Features

- Interactive dashboard with device-like status cards and module navigation
- Sub-GHz simulator with frequency presets, spectrum visualizer, signal capture and transmission
- NFC/RFID-style interface for card emulation and inspection workflows
- BadUSB script editor/execution mockup
- GPIO control panel for pin state simulation
- Infrared transmitter and code library layout
- iButton simulation panel
- BLE discovery and device interaction mockup
- Virtual file manager for Flipper-style storage browsing
- Dark theme and neon UI styling inspired by Flipper Zero tooling
- Client-side routing and a production-ready static build flow

## Tech Stack

- React 19
- TypeScript
- Vite
- Tailwind CSS
- Wouter for routing
- Recharts for charting
- Express for static asset serving
- PNPM for dependency management

## Project Structure

```text
.
├── client/
│   └── src/
│       ├── components/
│       ├── contexts/
│       ├── hooks/
│       ├── lib/
│       ├── pages/
│       ├── App.tsx
│       ├── const.ts
│       ├── index.css
│       └── main.tsx
├── server/
│   └── index.ts
├── shared/
├── patches/
├── package.json
├── pnpm-lock.yaml
├── tsconfig.json
├── tsconfig.node.json
├── vite.config.ts
├── components.json
├── ideas.md
└── .gitignore
```
## Getting Started

### Prerequisites

* Node.js 18+
* PNPM

### Install dependencies

```bash
pnpm install
```
### Run the app in development mode

```bash
pnpm dev
```

This starts the Vite development server with host access enabled.

### Build for production

```bash
pnpm build
```
This creates the production build and bundles the Express server entry in dist.

### Start the production server

```bash
pnpm start
```
The app is served via the Express server on port 3000 by default.

### Available Scripts

```bash
pnpm dev      # Start Vite dev server
pnpm build    # Build frontend + server bundle
pnpm start    # Run production app
pnpm preview  # Preview production build locally
pnpm check    # Type-check with TypeScript
pnpm format   # Format code with Prettier
```

## Notes

* The simulator is intentionally front-end focused and uses mock data and UI interactions rather than actual RF or hardware communication.
* The homepage in package.json points to a GitHub Pages deployment URL.
* The app includes a dark industrial UI theme and is optimized for browser demos and prototype exploration.

## License

This project is licensed under the MIT License.

## Contributing

Contributions are welcome. If you are improving the simulator, adding new modules, or polishing the UI, open a pull request with a clear description of the changes and the expected behavior.

## Demo / Deployment

The project is configured for GitHub Pages hosting and also includes a Node/Express production server for local serving.

## Why this project exists

Flipper Zero is a popular multi-tool device for radio, wireless, USB, and embedded experimentation. This project brings that experience into the browser so users can explore the interface, learn the system concepts, and prototype workflows without hardware constraints.

```Code
If you want, I can also tailor the README to a specific tone:
- project-focused
- marketing/demo-focused
- developer onboarding-focused
- concise GitHub-style README
```

# Install Infosourceful Desktop

> **Status:** Early documentation. This page will be updated as installers and packaging stabilize.

## Prerequisites

- A supported desktop OS (Windows, macOS, or Linux)
- Git installed (for development builds)
- Node.js + npm (for the desktop shell, if building from source)
- Python (for engine/core, if building from source)

## Development Install (from source)

Until there is a packaged installer, you can run Infosourceful Desktop in development mode:

1. **Clone the app repository**

   ```bash
   git clone https://github.com/Infosourceful/infosourceful-app.git
   cd infosourceful-app
   ```

2. **Install dependencies**

   ```bash
   # Example – adjust to your actual setup
   npm install
   ```

3. **Start the desktop app (dev mode)**

   ```bash
   npm run tauri dev
   ```

The app will open in a desktop window. From there you'll be able to open a bundle and explore artifacts.

As packaging and installers are finalized, this page will be updated with:

- Download links for platform-specific installers
- Checksums/signatures
- Upgrade instructions
- Troubleshooting steps


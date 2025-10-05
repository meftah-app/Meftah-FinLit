Meftah-FinLit — GitHub Upload Package

This package is prepared to upload into your empty GitHub repository:
https://github.com/meftah-app/Meftah-FinLit

Steps to upload:
1. Unzip this archive locally.
2. Preferred (git) method:
   git clone https://github.com/meftah-app/Meftah-FinLit.git
   cd Meftah-FinLit
   cp -R /path/to/unzipped/* .
   git add .
   git commit -m "Initial upload: Meftah FinLit"
   git push origin main

3. Alternatively, on GitHub repo page click "Upload files" and drag all files from this package.

After files are pushed:
- Go to Actions tab and watch the 'build-electron' workflow.
- After successful run, download installers from Artifacts:
  - Windows: NSIS installer (.exe)
  - macOS: DMG (.dmg)
  - Linux: AppImage (.AppImage)

Notes:
- To run the app locally without CI: build frontend (cd frontend && npm install && npm run build), then from project root run npm install and npm run dist (requires electron-builder and platform-specific environment).
- Seed data and test users are included; see backend/seed.js and README.

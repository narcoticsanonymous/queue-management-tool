# Queue Manager

A simple web-based queue management system for tracking participant status.

## Overview

This application provides a visual grid of 150 numbered participant buttons. Each participant can cycle through three states by clicking:

- **White**: Not in queue
- **Orange**: First queue state
- **Light blue**: Second queue state

## Usage

Simply open `index.html` in any web browser. No installation or build process required.

### Controls

- **Click any participant button**: Cycles through the three states (white → orange → light blue → white)
- **Reset button**: Returns all participants to the initial white state

## Technical Details

- Pure vanilla JavaScript (no dependencies)
- 150 participants by default (configurable in code)
- State tracked via HTML attributes

## Deployment to GitHub Pages

1. Create a new repository on GitHub
2. Add the remote and push:
   ```bash
   git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git push -u origin main
   ```
3. In your GitHub repository settings:
   - Go to **Settings** → **Pages**
   - Under **Source**, select **GitHub Actions**
4. The GitHub Action will automatically deploy on every push to main
5. Your site will be live at `https://YOUR-USERNAME.github.io/YOUR-REPO/`

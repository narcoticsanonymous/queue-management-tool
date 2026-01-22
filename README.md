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

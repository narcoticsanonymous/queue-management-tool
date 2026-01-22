# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a simple HTML/JavaScript application for managing participant queues. It creates a visual grid of numbered buttons representing participants (1-150), where each can cycle through three states:
- White (queue="0"): Not in queue
- Orange (queue="1"): First queue state
- Light blue (queue="2"): Second queue state

## Architecture

**Single-file application**: The entire application lives in `index.html` with embedded JavaScript.

**Dependencies**: None - uses vanilla JavaScript (no external libraries)

**State management**: Uses HTML attribute `queue` on button elements to track state (values: "0", "1", or "2")

**Core functionality**:
- Dynamically generates 150 participant buttons on page load using `createElement` and `appendChild`
- Click handler cycles each button through the three states
- Reset button returns all participants to initial white/queue="0" state

## Running the Application

Open `index.html` directly in a web browser. No build process, server, or dependencies to install.

## Key Implementation Details

The participant count is controlled by the `participants` constant, currently set to 150. Each button has an ID of `matrix{N}` where N is the participant number. Button styling is managed via a CSS class `.participant-button` for initial styling, with individual state colors applied inline.

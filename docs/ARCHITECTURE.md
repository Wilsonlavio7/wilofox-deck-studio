# Architecture

## Overview

Wilofox Deck Studio is a portable browser application implemented primarily in a single HTML file.

## Main components

- HTML5 interface
- CSS visual system
- Vanilla JavaScript application logic
- IndexedDB local persistence
- WebMCP tool registration
- Presenter and audience views

## Shared state

Manual actions and WebMCP tool calls use the same application state, rendering functions, and persistence layer.

The basic flow is:

1. A person or AI agent requests an action.
2. The application validates the input.
3. The shared deck state is updated.
4. The change is stored locally.
5. The visible interface is rendered again.

## Progressive enhancement

WebMCP is an additional capability. Browsers without WebMCP can continue using the complete manual editor and presentation experience.

## Project structure

- `dist/index.html`: complete browser application
- `.openai/hosting.json`: static hosting configuration
- `docs/`: project and testing documentation
- `LICENSE`: MIT open-source license

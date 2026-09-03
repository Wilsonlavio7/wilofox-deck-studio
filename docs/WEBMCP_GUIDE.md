# WebMCP Guide

## What is WebMCP?

WebMCP allows a website to expose structured actions that an AI agent can understand and use. The agent does not need to infer every action from buttons or screen coordinates.

Wilofox Deck Studio registers four tools through `document.modelContext.registerTool()`.

| Tool | Purpose |
|---|---|
| `create_deck` | Creates and opens an editable presentation |
| `get_deck_context` | Reads the latest deck state, including human edits |
| `update_slide` | Updates one requested slide while preserving the others |
| `navigate_to_slide` | Opens a requested slide for review |

## Browser status

When WebMCP is active, the application displays:

`WebMCP - 4 active tools`

If the browser is unsupported, it displays:

`WebMCP - unsupported browser`

## Suggested test

1. Open the live application in ChatGPT's in-app browser.
2. Ask the agent:

> Create a three-slide beginner presentation in Spanish titled "Safe AI in the classroom."

3. Manually change the title of slide 2.
4. Ask the agent:

> Read the latest deck state. Improve only slide 2, preserve my edited title, and leave every other slide unchanged.

5. Ask the agent to navigate to slide 2.

## Expected result

The agent should:

- Detect the current presentation.
- Preserve the manual edit.
- Modify only the requested slide.
- Display the result in the same visible interface.

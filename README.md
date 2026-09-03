# Wilofox Deck Studio · WebMCP

Wilofox Deck Studio is a single-file presentation studio for educators and creators. This WebMCP edition turns the existing human-first editor into a shared workspace where a person and an AI agent can create and refine the same visible deck.

## WebMCP tools

- `create_deck` — creates a new structured presentation and opens it in the editor.
- `get_deck_context` — reads the latest deck state, including human edits.
- `update_slide` — changes one requested slide while preserving the rest of the deck.
- `navigate_to_slide` — brings a requested slide into view for joint review.

Every tool uses the same application state and render functions as the manual editor. The application remains fully functional in browsers without WebMCP; agent support is a progressive enhancement.

## Test WebMCP

Open the deployed app in ChatGPT's in-app browser. In supported Google Chrome builds, enable `chrome://flags/#enable-webmcp-testing` and relaunch the browser.

Example request to an agent:

> Create a 5-slide beginner deck about prompt engineering. Include a concrete example and a final knowledge check. Then show me slide 2.

## Run locally

Serve `dist/` from a local HTTP server and open `index.html`.

## License

MIT

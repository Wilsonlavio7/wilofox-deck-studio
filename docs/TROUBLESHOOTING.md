# Troubleshooting

## WebMCP reports an unsupported browser

1. Use ChatGPT's in-app browser or a compatible Chrome build.
2. In supported Chrome versions, open:

   `chrome://flags/#enable-webmcp-testing`

3. Set **WebMCP for testing** to **Enabled**.
4. Completely relaunch Chrome.
5. Open the live application again.
6. Use `Ctrl + Shift + R` to reload it.

## The library is empty

Select **Load example** or create a new presentation.

## The AI agent cannot see the tools

Confirm that the application displays:

`WebMCP - 4 active tools`

If it does not, relaunch the compatible browser and reload the application.

## Changes are not visible

Navigate back to the requested slide or reload the current presentation.

## Important data note

Presentation data is stored locally in IndexedDB. Export important work before clearing browser storage or site data.

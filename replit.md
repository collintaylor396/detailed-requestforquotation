# Running and publishing

This is a plain HTML site. `index.html` immediately redirects visitors to
`https://www.google.com`, preserving the URL fragment (the text after `#`).
There are no dependencies, secrets, or external services to configure.

## Preview

Use the **Start application** workflow. It copies `index.html` into `dist/`
and serves that directory with Python's development server on port 5000.
Only the HTML page is served, not workspace configuration or repository files.

## Publish

The project uses Static publishing. Its build command is
`mkdir -p dist && cp index.html dist/index.html`, and its public directory is
`dist`. Click **Publish** to make the page live.
Python is only used for local preview; the published page needs no server.
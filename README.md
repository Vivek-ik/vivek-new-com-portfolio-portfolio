Vivek — How to run this project locally

This is a simple static HTML/CSS/JS template (no build step). Use any static file server or open files directly in your browser.

Quick options (PowerShell commands)

1) Open directly in the browser
- In File Explorer, double-click `index.html` to open it in your default browser.

2) Start a simple HTTP server with Python 3 (recommended if you have Python installed)
- From the project root in PowerShell:

```powershell
python -m http.server 8000
# then open http://localhost:8000 in your browser
```

3) Use Node's `http-server` (if you have Node.js + npm)

```powershell
npm install -g http-server
# from project root
http-server -p 8000
# then open http://localhost:8000
```

4) Use VS Code Live Server extension (recommended for editing)
- Install the Live Server extension in VS Code.
- Open this folder in VS Code, open `index.html`, and click "Go Live" (bottom-right). It will serve the site and live-reload on changes.

Stopping servers
- Python: Ctrl+C in the PowerShell window running `python -m http.server`.
- http-server: Ctrl+C in that terminal as well.

Notes and useful details
- This template is a static site — there are no build steps, package.json, or server-side code.
- Mailchimp form: the original template includes a Mailchimp example. See `readme.txt` for instructions to replace the MailChimp URL in `js/main.js` (search for `mailChimpURL`).
- Attribution: The template is from styleshout.com and the `readme.txt` contains license/attribution requirements. Keep the footer credit if required.

Troubleshooting
- If images/CSS don't load when opening the file directly, use a local HTTP server (browser blocks some resources for file://).
- If `python` command is not found on Windows, try `py -3 -m http.server 8000`.
- If ports are in use, try a different port (e.g., `8001`).

Want me to add a one-click npm script, a package.json, or a GitHub Pages deploy guide? Tell me which you'd prefer and I can add it.

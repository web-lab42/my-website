# Security notes

- Static client-side app: no server, API, credentials, cookies, local storage, analytics, or outbound application requests.
- No third-party scripts, fonts, stylesheets, or runtime dependencies.
- Dynamic log content is rendered with DOM `textContent` / node creation rather than interpolating user-provided strings into HTML.
- Do not add secrets to this repository.
- GitHub Pages provides static hosting only; it cannot enforce hidden game state. The bomb layout is discoverable by a user with access to the browser runtime/source.
- This document describes design intent, not a formal security audit or guarantee.

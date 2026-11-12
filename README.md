# qb-oauth-callback

Static bridge page for the OAuth 2.0 redirect of an internal QuickBooks Online integration.
Intuit requires production redirect URIs to be served from a web server, so this page receives
the redirect and forwards the query string unchanged to the local listener
(`https://localhost:8765/callback`) on the machine that started the authorization.
It stores nothing and calls nothing else.

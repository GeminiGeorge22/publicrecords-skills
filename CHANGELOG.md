## 1.4.0

- Add five skills for the new public Actors: `pdf-to-text` (`pdf-docx-to-markdown`), `audio-to-text` (`audio-file-transcriber`), `web-page-to-markdown` (`url-to-markdown`), `js-page-to-markdown` (`js-page-to-markdown`), and `email-verifier` (`email-verifier`).
- Email Verifier is described as a domain, MX and disposable-domain check, not a mailbox or SMTP check. No mail is sent.
- Add those five Actors to the fleet Apify MCP `?tools=` list used by the skills and client manifests (runs still bill the user's own Apify account).

## 1.3.0

- Add `tennis-scores` skill for `publicrecords/tennis-scores-api`. The skill calls the Actor through the Apify API with the user's own token. Standby/MCP mode is not built, so this Actor is not added to the fleet MCP `?tools=` list.

## 1.2.0

- Add a Cursor project rule (`.cursor/rules/publicrecords-apify.mdc`) and `.cursor-plugin/plugin.json`.
- Document OpenCode, Cline, Roo and Kilo installs under `docs/`, including that Actor runs use the user's own Apify token.

# Changelog

## 1.1.0 (2026-11-23)

- Add `skool-communities` skill for `publicrecords/skool-community-growth-tracker`.
- Include that Actor on the fleet Apify MCP `?tools=` list used by all skills and client manifests.

## 1.0.0 (2026-11-23)

- First release: 8 Agent Skills covering 17 publicrecords Actors; Agent Plugins, Claude Code, Codex, Gemini CLI manifests; hosted Apify MCP config.

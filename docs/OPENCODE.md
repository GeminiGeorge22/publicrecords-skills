# OpenCode

Public Records skills are standard Agent Skills (`SKILL.md`). OpenCode loads them the same way other skills clients do. Actor runs bill **your own** Apify account. This repository has no tokens.

## Install the skills

From a project, or for your user install:

```bash
npx skills add GeminiGeorge22/publicrecords-skills
```

OpenCode discovers `skills/*/SKILL.md` after that install. You can also clone the repo and point OpenCode at the `skills/` directory. OpenCode V1 and V2 both work with these files; there is no OpenCode-only plugin binary.

## Optional: hosted MCP

If you want live Actor runs from the same session, add the hosted Apify MCP server and sign in with your Apify account (OAuth, or `Authorization: Bearer` plus **your** API token):

```json
{
  "mcp": {
    "publicrecords": {
      "type": "remote",
      "url": "https://mcp.apify.com/?tools=publicrecords/company-social-profile-finder,publicrecords/govcon-opportunity-feed,publicrecords/grants-gov-scraper,publicrecords/usaspending-awards-scraper,publicrecords/uk-find-a-tender-scraper,publicrecords/eu-ted-notices-scraper,publicrecords/legistar-meetings-scraper,publicrecords/ashby-jobs-scraper,publicrecords/greenhouse-jobs-scraper,publicrecords/lever-jobs-scraper,publicrecords/smartrecruiters-jobs-scraper,publicrecords/etsy-search-scraper,publicrecords/etsy-shop-velocity,publicrecords/google-ads-transparency-scraper,publicrecords/sports-odds-api,publicrecords/spotify-play-count-scraper,publicrecords/calibration-ledger"
    }
  }
}
```

If your OpenCode build expects a different MCP key shape, keep the URL and auth the same and follow [OpenCode MCP docs](https://opencode.ai/docs/mcp-servers/).

## What you can ask

Examples, each of which routes to one Actor:

- Which IT services contracts were posted on SAM.gov in the last 14 days?
- What jobs did Ramp post on Ashby this week?
- Find the official LinkedIn page for hubspot.com.
- How did this Etsy shop's sales look over the last 28 days?

Author: Public Records (https://apify.com/publicrecords).

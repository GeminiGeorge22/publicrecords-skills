# Cline, Roo and Kilo

These skills and the hosted MCP server work in Cline, Roo Code and Kilo Code the same way they work in other Agent Skills / MCP clients. Actor runs bill **your own** Apify account. This repository has no tokens.

## Skills

```bash
npx skills add GeminiGeorge22/publicrecords-skills
```

Cline also accepts `cline skill install GeminiGeorge22/publicrecords-skills`. Kilo reads the same `SKILL.md` folders.

## MCP

Paste this into the client's MCP settings. Sign in with your Apify account (OAuth or `Authorization: Bearer` plus **your** API token):

```json
{
  "mcpServers": {
    "publicrecords": {
      "type": "http",
      "url": "https://mcp.apify.com/?tools=publicrecords/company-social-profile-finder,publicrecords/govcon-opportunity-feed,publicrecords/grants-gov-scraper,publicrecords/usaspending-awards-scraper,publicrecords/uk-find-a-tender-scraper,publicrecords/eu-ted-notices-scraper,publicrecords/legistar-meetings-scraper,publicrecords/ashby-jobs-scraper,publicrecords/greenhouse-jobs-scraper,publicrecords/lever-jobs-scraper,publicrecords/smartrecruiters-jobs-scraper,publicrecords/etsy-search-scraper,publicrecords/etsy-shop-velocity,publicrecords/google-ads-transparency-scraper,publicrecords/sports-odds-api,publicrecords/spotify-play-count-scraper,publicrecords/calibration-ledger"
    }
  }
}
```

Author: Public Records (https://apify.com/publicrecords).

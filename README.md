# Citation Safe MCP

Deterministic verification of legal citations — existence, quote-match, and proposition-support checks against primary sources (CourtListener, USCourts.gov). Not LLM guessing.

**Transport:** Streamable HTTP
**Endpoint:** `https://citationsafe.com/api/mcp`
**Docs:** https://citationsafe.com/mcp
**Category:** Legal / Verification
**Free tier:** 5 checks/day per IP, no signup

## Tools
- `is_this_case_real` — single-citation existence check (free/anonymous)
- `verify_brief` — multi-citation existence + quote check (free/anonymous)
- `verify_citation` — 3-layer verification (adds proposition support on paid tiers)
- `verify_document` — same, fetches URL (auth required)
- `search_sanctions` — search real AI-hallucination sanction orders
- `search_phantoms` — search known fabricated (phantom) citations
- `batch_verify_citations`, `get_verification`

## Client config (Claude Desktop / Cursor)
```json
{
  "mcpServers": {
    "citation-safe": { "url": "https://citationsafe.com/api/mcp" }
  }
}
```

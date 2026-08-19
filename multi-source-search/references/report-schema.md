# Research report schema

Save the research ledger as one UTF-8 JSON object:

```json
{
  "question": "What is being investigated?",
  "searched_at": "2026-08-15",
  "providers": ["host_web_search", "host_page_open", "scholar_search_mixed"],
  "unavailable_providers": [],
  "sources": [
    {
      "id": "s1",
      "url": "https://example.org/primary-study",
      "publisher": "Example Institute",
      "source_type": "primary"
    }
  ],
  "claims": [
    {
      "id": "c1",
      "text": "A bounded, checkable claim.",
      "kind": "sourced",
      "confidence": "low",
      "source_ids": ["s1"],
      "independent_source_count": 1,
      "conflict": false
    }
  ],
  "gaps": ["Independent replication is not available."]
}
```

Rules:

- Record the actual capability names used, including native host tools. Record at least
  two unique capabilities; repeated queries to one capability still count as one. List
  unavailable capabilities separately.
- Source IDs and URLs must be unique. Source type is `primary`, `secondary`, or `aggregator`.
- Claims reference existing source IDs and declare `kind` as `sourced` or `inference`.
- High confidence requires at least three independent sources; medium requires two; low requires one.
- A conflicting claim cannot be high confidence.
- Every source must support at least one claim, and every evidence gap must be explicit.

The validator does not fetch URLs, judge credibility, detect hidden shared sources, or prove claims true.

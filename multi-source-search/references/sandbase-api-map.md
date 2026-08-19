# SandBase Multi-Source Search API Map

Use these tools through the SandBase gateway. Before each call, use `sandbase_describe_tool` to obtain current parameters, then use `sandbase_call_tool` with the exact tool name.

| Tool name | Use it for |
|---|---|
| `tavily_search` | Current web search with depth and topic control. |
| `tavily_extract` | Extract clean content from URLs. |
| `exa_search` | Semantic search for high-quality sources. |
| `exa_contents` | Extract content from Exa results. |
| `scholar_search_mixed` | Academic + web combined search. |
| `scholar_search_scholar` | Pure academic search. |
| `scholar_search_web` | Web search with academic lens. |
| `cloudsway_search` | Broad web search coverage. |

Use multiple sources for cross-validation. Score confidence by source agreement.

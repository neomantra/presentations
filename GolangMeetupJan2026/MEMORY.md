# Memory Notes for Presentation Development

## MCP Agent Looping Slide (May 2025)

### Key Narrative Arc
The slide should capture the "aha moment" - realizing that the bottleneck isn't the tool's power, but how well you describe it to the LLM, and you can use the LLM to help you do that.

### Research Sources
- [screentime-mcp GitHub](https://github.com/AgentDank/screentime-mcp)
- [Tool description file](https://github.com/AgentDank/screentime-mcp/blob/main/internal/mcp/screentime_sql.tooldesc.md)
- HN comment: "I've found good value in making purpose-built MCP servers... with verbose description for the LLM of an 'sql' tool endpoint for it to use to explore"

### Suggested Content

**Title options:**
- "MCP Agent Looping" (current)
- "The Agent Loop Epiphany"
- "Tool Descriptions Matter"

**Bullet points:**
- Built [screentime-mcp](https://github.com/AgentDank/screentime-mcp) — query macOS Screen Time via SQL
- Pattern: Data → DuckDB → MCP → LLM (with verbose tool descriptions)
- Agent loop: Claude queries → fails → informs better descriptions → self-corrects
- Use the LLM itself to write better tool descriptions
- Detailed markdown docs of schema, views, query patterns
- Returns CSV — easier for LLM to parse

**Takeaway box:**
"The bottleneck isn't tool power — it's tool description quality. Use the LLM to help write verbose, structured documentation that enables autonomous exploration."

**Presenter notes (with Crush anecdote for longer talks):**
"This is where the pattern crystallized. I built screentime-mcp to query my Mac's Screen Time data through SQL. The key insight: Claude would fail on queries, and those failures told me exactly how to improve the tool descriptions. Better descriptions led to Claude self-correcting. And here's the meta part — I used Claude to help write those tool descriptions based on the failure modes it encountered. I was also using Charmbracelet Crush to develop this while improving Crush's MCP support. The pattern Data→DuckDB→MCP→LLM with verbose SQL endpoint descriptions became my go-to architecture."

### Technical Details from screentime-mcp
- Queries macOS Screen Time from `knowledgeC.db` (requires Full Disk Access)
- Loads into DuckDB, exposes single `screentime_sql` endpoint
- Returns CSV for easier LLM parsing
- Apple timestamps are seconds since 2001-01-01 (needs 31-year adjustment)
- Core tables: ZOBJECT (events), ZSTRUCTUREDMETADATA (metadata), ZSOURCE (apps)

# Contributing to Awesome MCP Hub

We welcome contributions from the community! Whether you're submitting a new server, improving descriptions, or fixing errors, your help is appreciated.

## How to Submit a Server

### For the Curated Section

Curated servers are hand-picked by our editors for quality, reliability, and usefulness. To nominate a server:

1. Open an [Issue](../../issues/new?template=curated-nomination.md) with the "Curated Nomination" template
2. Include:
   - Server name and repository URL
   - Why it deserves curated status (quality, unique features, active maintenance)
   - Your experience using it
3. Our editors will review, test, and decide on inclusion

**Curated criteria:**
- Actively maintained (commits within last 3 months)
- Well-documented README with clear setup instructions
- Works reliably with at least 2 MCP clients
- Solves a real problem or provides unique value
- Has proper error handling and doesn't crash

### For the Community Section

Community servers are open to all contributions via pull request:

1. **Fork** this repository
2. **Add** your server to the appropriate category in `README.md`
3. **Follow** the entry format (see below)
4. **Submit** a pull request

### Entry Format

```markdown
| [Server Name](https://github.com/owner/repo) | Brief description of what it does (max 120 chars) | `npx command` or setup instructions | Language | Difficulty |
```

**Fields:**
- **Server Name**: Link to the repository
- **Description**: Concise, factual description (no marketing language)
- **Install**: Primary install command
- **Language**: Implementation language icon (see legend)
- **Difficulty**: Setup difficulty level

### Difficulty Levels

| Level | Meaning |
|-------|---------|
| Easy | One command setup (`npx`, `pip install`) |
| Medium | Requires configuration (API keys, config files) |
| Advanced | Requires infrastructure (Docker, databases, cloud services) |

## Guidelines

- **Alphabetical order** within each category
- **One server per row** in the table
- **Accurate information** — test the install command before submitting
- **No duplicates** — search the list first
- **No spam** — servers must provide genuine value
- **Working links** — all URLs must be accessible

## Updating Existing Entries

If you notice outdated information, broken links, or missing features, please submit a PR with the fix.

## Reporting Issues

Found a broken server or incorrect information? [Open an issue](../../issues/new) and we'll fix it.

Thank you for contributing!

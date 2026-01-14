# Cowork Capabilities (Verified)

> **Source Verification**: All capabilities listed here are confirmed by official Anthropic announcements or independent testing from trusted sources.

## Verified Capabilities

### 1. Local File Access

**Source**: [TechCrunch](https://techcrunch.com/2026/01/12/anthropics-new-cowork-tool-offers-claude-code-without-the-code/), [Simon Willison](https://simonwillison.net/2026/Jan/12/claude-cowork/)

| Operation | Verified | Notes |
|-----------|----------|-------|
| Read files | Yes | Within designated folders only |
| Create files | Yes | New files in accessible folders |
| Modify files | Yes | Edit existing files |
| Move files | Yes | Between accessible locations |
| Rename files | Yes | Batch renaming supported |
| Delete files | Yes | **Use with caution** |

### 2. Multi-Step Task Execution

**Source**: [TechCrunch](https://techcrunch.com/2026/01/12/anthropics-new-cowork-tool-offers-claude-code-without-the-code/)

> "Multi-step task execution without requiring user input between actions"

- Claude breaks complex tasks into steps
- Executes sequentially without prompting
- Reports progress during execution

### 3. Sandboxed Environment

**Source**: [Simon Willison](https://simonwillison.net/2026/Jan/12/claude-cowork/)

- Uses Apple's VZVirtualMachine for containerization
- Files are mounted into the sandbox
- Cannot access files outside designated folders
- Isolation prevents system-wide access

## Verified Use Cases

Based on official sources:

| Use Case | Source | Verified |
|----------|--------|----------|
| File organization | TechCrunch | Yes |
| Expense reports from receipts | TechCrunch | Yes |
| Media file management | TechCrunch | Yes |
| Content analysis | Simon Willison | Yes (tested with 46 files) |
| Research across files | Simon Willison | Yes |

## NOT Verified (Removed)

The following claims appeared in early documentation but are **not confirmed** by official sources:

- Excel spreadsheet creation with formulas
- PowerPoint presentation generation
- Word document creation
- "Zero timeout" execution
- "Parallel workstream" coordination

*These may be possible but are not documented in verified sources.*

## Technical Architecture

```
┌─────────────────────────────────────────┐
│            Claude Desktop App            │
└─────────────────────────────────────────┘
                    │
                    ▼
┌─────────────────────────────────────────┐
│          Cowork Mode Selector            │
└─────────────────────────────────────────┘
                    │
                    ▼
┌─────────────────────────────────────────┐
│    VZVirtualMachine Sandbox Container    │
│    - Mounted folder access only          │
│    - Isolated from system files          │
└─────────────────────────────────────────┘
                    │
                    ▼
┌─────────────────────────────────────────┐
│         Your Designated Folder           │
└─────────────────────────────────────────┘
```

## Browser Integration

**Source**: [TechCrunch](https://techcrunch.com/2026/01/12/anthropics-new-cowork-tool-offers-claude-code-without-the-code/)

When paired with **Claude in Chrome** extension:
- Can complete tasks requiring web access
- Research and verification tasks
- Combined local + web workflows

## Security Model

**Source**: [Simon Willison](https://simonwillison.net/2026/Jan/12/claude-cowork/)

| Security Feature | Status |
|------------------|--------|
| Sandboxed execution | Yes |
| Folder-level permissions | Yes |
| Prompt injection mitigations | Active development |
| User confirmation for destructive actions | Recommended |

### Anthropic's Warnings

1. Prompt injection remains a risk
2. Accidental file deletion possible
3. Sensitive data should not be accessible
4. Research preview - not production ready

---

*Last verified: January 13, 2026*
*Sources: TechCrunch, Simon Willison, VentureBeat*

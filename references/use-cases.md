# Cowork Use Cases (Verified)

> **Important**: Only use cases confirmed by official sources or independent testing are included here.

## Tier 1: Officially Confirmed

These use cases are mentioned in Anthropic's official communications or verified tech press:

### File Organization

**Source**: [TechCrunch](https://techcrunch.com/2026/01/12/anthropics-new-cowork-tool-offers-claude-code-without-the-code/)

```
"Sort all the PDFs in my Downloads folder by date and move them to appropriate subfolders"
```

```
"Organize my documents by file type into separate folders"
```

### Expense Reports

**Source**: [TechCrunch](https://techcrunch.com/2026/01/12/anthropics-new-cowork-tool-offers-claude-code-without-the-code/)

> "Assembling expense reports from receipt photos"

```
"Go through the receipt photos in this folder and create a summary of expenses"
```

### Media Management

**Source**: [TechCrunch](https://techcrunch.com/2026/01/12/anthropics-new-cowork-tool-offers-claude-code-without-the-code/)

> "Managing media files"

```
"Organize my photos by month and year into separate folders"
```

## Tier 2: Independently Tested

These use cases were tested by trusted independent sources:

### Content Analysis

**Source**: [Simon Willison](https://simonwillison.net/2026/Jan/12/claude-cowork/)

Simon tested with 46 draft files:

```
"Identify all draft files modified in the last 90 days and check which ones are ready for publication"
```

**Result**: Claude successfully:
- Located 46 relevant files
- Executed 44 web searches to verify publication status
- Provided actionable recommendations

### Research Tasks

**Source**: [Simon Willison](https://simonwillison.net/2026/Jan/12/claude-cowork/)

```
"Search through these files and identify patterns"
```

```
"Analyze these text files and create a summary of findings"
```

## Tier 3: Mentioned but Not Detailed

These appear in coverage but without specific verification:

- Scanning social media posts
- Analyzing conversations
- General file search and categorization

## What NOT to Expect (Unverified)

The following were **removed** from documentation due to lack of verification:

| Claim | Status | Why Removed |
|-------|--------|-------------|
| Excel with formulas | Unverified | No official source confirms this |
| PowerPoint creation | Unverified | No official source confirms this |
| Word document formatting | Unverified | No official source confirms this |
| Parallel task execution | Unverified | Language was marketing, not technical |

## Best Practices for Tasks

### DO: Be Specific

```
GOOD: "Sort PDFs in Downloads by date, creating folders for 2024, 2025, 2026"

BAD: "Clean up my files"
```

### DO: Start Small

Test with non-critical folders first:

```
"List all files in this test folder and tell me what you see"
```

### DO: Provide Context

```
"These are receipt photos from business travel. Create a summary with date, vendor, and amount for each."
```

### DON'T: Assume Complex Outputs

Until verified, don't assume Claude can:
- Create formatted spreadsheets with formulas
- Generate presentation slides
- Produce complex formatted documents

## Security Reminders

Before any task:

1. **Back up important files** - Mistakes can happen
2. **Start with read-only tasks** - Test before modifying
3. **Avoid sensitive folders** - No passwords, keys, or credentials
4. **Be specific** - Ambiguous instructions can cause unexpected behavior

---

*Last verified: January 13, 2026*
*Only includes use cases from verified sources*

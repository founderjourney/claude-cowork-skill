<p align="center">
  <img src="https://img.shields.io/badge/Claude-Cowork-5A45FF?style=for-the-badge&logo=anthropic&logoColor=white" alt="Claude Cowork"/>
  <img src="https://img.shields.io/badge/Status-Research%20Preview-orange?style=for-the-badge" alt="Status"/>
  <img src="https://img.shields.io/badge/Platform-macOS-000000?style=for-the-badge&logo=apple&logoColor=white" alt="Platform"/>
</p>

<h1 align="center">Claude Cowork Skill</h1>

<p align="center">
  <strong>Claude Code for the rest of your work.</strong><br/>
  <em>File access and automation through natural language - no coding required.</em>
</p>

<p align="center">
  <a href="#what-is-cowork">What is Cowork?</a> •
  <a href="#verified-capabilities">Capabilities</a> •
  <a href="#requirements">Requirements</a> •
  <a href="#installation">Install</a>
</p>

---

> **Research Preview**: Cowork launched January 12, 2026. Anthropic warns about prompt injection risks and accidental file operations. Use with caution.

---

## What is Cowork?

Anthropic describes Cowork as **"Claude Code for the rest of your work"** - it extends agentic capabilities to non-developers.

Instead of explaining how to organize files, Claude does it.

```
You: "Sort my Downloads by file type into separate folders"

Claude: *actually does it*
```

**How it's described by TechCrunch:**
> "A sandboxed instance of Claude Code, but requires far less technical savvy to set up."

---

## Verified Capabilities

Based on [official announcements](https://techcrunch.com/2026/01/12/anthropics-new-cowork-tool-offers-claude-code-without-the-code/) and [independent testing](https://simonwillison.net/2026/Jan/12/claude-cowork/):

| Capability | Status | Source |
|------------|--------|--------|
| Read files in designated folders | Verified | TechCrunch, Simon Willison |
| Modify/create files | Verified | TechCrunch |
| Multi-step task execution | Verified | TechCrunch |
| File organization (sort, move, rename) | Verified | Multiple sources |
| Expense reports from receipts | Verified | TechCrunch |
| Content analysis across files | Verified | Simon Willison tested with 46 files |

### What's NOT verified (removed from this skill):
- Excel with formulas creation
- PowerPoint generation
- "Zero timeout" execution
- "Parallel workstreams"

*We only document what's been confirmed by official sources or independent testing.*

---

## How It Works

1. **Designate a folder** - You choose what Claude can access
2. **Sandboxed execution** - Runs in Apple's VZVirtualMachine container
3. **Natural language tasks** - Describe what you want done
4. **Results in your folder** - Output appears where you specified

```
┌─────────────────────────────────────────┐
│          YOUR DESIGNATED FOLDER          │
└─────────────────────────────────────────┘
                    │
                    ▼
┌─────────────────────────────────────────┐
│     SANDBOXED CONTAINER ENVIRONMENT      │
│   (Files mounted, isolated execution)    │
└─────────────────────────────────────────┘
                    │
                    ▼
┌─────────────────────────────────────────┐
│            TASK COMPLETED ✓              │
└─────────────────────────────────────────┘
```

---

## Requirements

| Requirement | Details |
|-------------|---------|
| **Platform** | macOS only (Windows planned) |
| **Subscription** | Claude Max required ($100-200/month) |
| **App** | Claude Desktop must remain open |
| **Connection** | Active internet required |

---

## Security Warnings

Anthropic explicitly warns about:

1. **Prompt Injection** - Files could contain malicious instructions
2. **Accidental Deletion** - Claude can delete files if misunderstanding instructions
3. **Sensitive Data** - Don't grant access to folders with passwords or keys

**Best Practices:**
- Start with non-critical folders
- Provide clear, unambiguous instructions
- Back up important files first
- Review actions before confirming destructive operations

---

## Verified Use Cases

### File Organization
```
"Sort all PDFs in Downloads by date into year folders"
```

### Expense Compilation
```
"Go through receipt photos and create an expense summary"
```

### Content Analysis
```
"Find all draft files modified in last 90 days and identify which are ready"
```
*This exact task was [tested by Simon Willison](https://simonwillison.net/2026/Jan/12/claude-cowork/) with 46 files successfully.*

### Media Management
```
"Organize photos by month and year into separate folders"
```

---

## Installation

### For Claude Code Users

```bash
# Clone this skill
git clone https://github.com/founderjourney/claude-cowork-skill.git ~/.claude/skills/cowork-complete
```

### Skill Structure

```
cowork-complete/
├── SKILL.md              # Skill definition (verified claims only)
├── README.md             # This file
└── references/
    ├── getting-started.md
    ├── capabilities.md
    └── use-cases.md
```

---

## Current Limitations

| Limitation | Details |
|------------|---------|
| macOS Only | Windows support announced but not available |
| Max Plan Only | $100-200/month subscription required |
| Research Preview | Features may change |
| No Projects | Cannot access Claude Projects |
| No Memory | No cross-session memory |
| App Must Stay Open | Tasks stop if closed |

---

## Sources & References

- [TechCrunch: Anthropic's new Cowork tool](https://techcrunch.com/2026/01/12/anthropics-new-cowork-tool-offers-claude-code-without-the-code/)
- [Simon Willison: First impressions of Claude Cowork](https://simonwillison.net/2026/Jan/12/claude-cowork/)
- [VentureBeat: Anthropic launches Cowork](https://venturebeat.com/technology/anthropic-launches-cowork-a-claude-desktop-agent-that-works-in-your-files-no)
- [Official Getting Started Guide](https://support.claude.com/en/articles/13345190-getting-started-with-cowork)

---

<p align="center">
  <sub>Skill packaged by <a href="https://github.com/founderjourney">Pathfinders Labs</a> from verified sources.</sub><br/>
  <sub>Claude Cowork is a research preview feature by Anthropic. Capabilities may change.</sub><br/>
  <sub>Last verified: January 13, 2026</sub>
</p>

---
name: cowork
description: Claude Cowork - Agentic file access for Claude Desktop. Read, modify, and organize files through natural language (research preview).
version: 1.1.0
author: Anthropic (skill packaged by Pathfinders Labs)
triggers:
  - cowork
  - Claude Desktop tasks
  - file automation
  - file organization
---

# Cowork Skill

Claude Cowork brings agentic capabilities to Claude Desktop, enabling Claude to work with files on your computer through natural language. Instead of explaining how to do tasks, Claude can execute them directly.

> **Important**: Cowork is a **research preview**. Anthropic warns about risks including prompt injection and accidental file operations. Use with caution and provide clear, unambiguous instructions.

## When to Use This Skill

Activate this skill when:
- User asks about **Cowork** features or setup
- User wants to automate **file organization** tasks
- User needs **multi-step file operations**
- User asks about **Claude Desktop agentic mode**

## What is Cowork?

Cowork is described by Anthropic as "Claude Code for the rest of your work" - it extends agentic capabilities to non-developers. Key concept:

> "A sandboxed instance of Claude Code, but requires far less technical savvy to set up." - TechCrunch

## Core Capabilities (Verified)

### 1. Local File Access
- Claude reads and modifies files within designated folders
- Files are mounted into a sandboxed container environment
- You choose which folders Claude can access

### 2. Multi-Step Task Execution
- Executes complex tasks without requiring user input between actions
- Breaks work into smaller steps automatically
- Reports progress during execution

### 3. Verified Use Cases
Based on official sources and independent testing:
- **File organization**: Sort, move, rename files by criteria
- **Expense reports**: Assemble reports from receipt photos
- **Media management**: Organize photos, documents, media files
- **Content analysis**: Scan and analyze text files, identify patterns
- **Research tasks**: Search and categorize information across files

## How It Works

1. You designate a folder for Claude to access
2. Claude operates within a sandboxed virtual environment (Apple's VZVirtualMachine)
3. Files are mounted into the container
4. Claude executes tasks through natural language instructions
5. Results appear in your designated folder

## Requirements

| Requirement | Details |
|-------------|---------|
| App | Claude Desktop (macOS only currently) |
| Plan | **Max subscription required** ($100-200/month) |
| Connection | Active internet required |
| State | App must remain open during execution |

## Getting Started

1. Open **Claude Desktop** app
2. Locate the **mode selector**
3. Click the **Cowork tab**
4. Select a folder to grant access
5. Assign Claude a task with clear instructions

## Example Tasks (Verified Working)

### File Organization
```
"Sort all the PDFs in my Downloads folder by date and move them to appropriate subfolders"
```

### Expense Compilation
```
"Go through the receipt photos in this folder and create a summary of expenses"
```

### Content Analysis
```
"Identify all draft files modified in the last 90 days and check which ones are ready for publication"
```

### Media Management
```
"Organize my photos by month and year into separate folders"
```

## Current Limitations

| Limitation | Description |
|------------|-------------|
| macOS Only | Windows support planned but not available |
| Max Plan Only | Not available on Pro or free plans |
| Research Preview | Features may change, not production-ready |
| No Projects | Cannot access Claude Projects |
| No Memory | No cross-session memory |
| App Must Stay Open | Tasks stop if you close the app |

## Security Considerations

Anthropic explicitly warns users about:

1. **Prompt Injection Risk**: Files you give Claude access to could contain malicious instructions
2. **Accidental Deletion**: Claude can delete files if instructed (or misunderstanding instructions)
3. **Sensitive Data**: Do not give access to folders with passwords, keys, or sensitive information

**Best Practices:**
- Start with non-critical folders to test
- Provide clear, unambiguous instructions
- Review Claude's actions before confirming destructive operations
- Back up important files before granting access

## Browser Integration

When paired with **Claude in Chrome** extension, Cowork can complete tasks requiring browser access for research and verification.

## Resources

- [TechCrunch Announcement](https://techcrunch.com/2026/01/12/anthropics-new-cowork-tool-offers-claude-code-without-the-code/)
- [Simon Willison's First Impressions](https://simonwillison.net/2026/Jan/12/claude-cowork/)
- [Getting Started Guide](https://support.claude.com/en/articles/13345190-getting-started-with-cowork)
- [Claude Desktop Download](https://claude.com/download)

---

*Skill packaged by Pathfinders Labs from verified sources. Last updated: January 13, 2026.*
*This is documentation for a research preview feature. Capabilities may change.*

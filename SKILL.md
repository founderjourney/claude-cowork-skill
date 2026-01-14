---
name: cowork
description: Claude Cowork - Agentic productivity capabilities for Claude Desktop that enable file access, multi-task coordination, and extended execution.
version: 1.0.0
author: Anthropic (skill packaged by Pathfinders Labs)
triggers:
  - cowork
  - Claude Desktop tasks
  - agentic productivity
  - file automation
  - multi-task coordination
---

# Cowork Skill

Claude Cowork brings agentic capabilities to Claude Desktop, enabling Claude to take on complex, multi-step tasks and execute them autonomously. Instead of responding to prompts one at a time, Claude can work independently on your behalf.

## When to Use This Skill

Activate this skill when:
- User asks about **Cowork** features or setup
- User wants to automate **file organization** tasks
- User needs **multi-task coordination** (parallel workstreams)
- User wants to create **professional documents** (Excel, PowerPoint)
- User asks about **Claude Desktop agentic mode**
- User needs **extended execution** tasks without timeouts

## What is Cowork?

Cowork is a research preview feature that extends Claude's agentic capabilities beyond coding to general productivity work. Key concept:

> "Give Claude access to your files and let it organize, create, and edit documents while you focus on what matters."

## Core Capabilities

### 1. Local File Access
- Claude reads and writes files directly on your computer
- No manual uploads or downloads required
- Works with a designated folder you choose

### 2. Multi-Task Coordination
- Breaks complex work into smaller subtasks
- Coordinates parallel workstreams
- Queue multiple tasks for execution

### 3. Professional Outputs
- Excel spreadsheets with formulas
- PowerPoint presentations
- Formatted Word documents
- Organized file structures

### 4. Extended Execution
- Handles complex tasks without conversation timeouts
- Works independently while you focus elsewhere
- Reports progress and completion

## How It Works

Cowork executes tasks through a 5-step process:

1. **Analyze** - Understanding your request
2. **Plan** - Breaking work into subtasks
3. **Execute** - Running in virtual machine environment
4. **Coordinate** - Managing parallel workstreams
5. **Deliver** - Outputs to your file system

## Requirements

| Requirement | Details |
|-------------|---------|
| App | Claude Desktop (macOS only) |
| Plan | Max subscription required |
| Connection | Active internet required |
| State | App must remain open during execution |

## Getting Started

1. Open **Claude Desktop** app
2. Locate the **mode selector**
3. Click the **Cowork tab**
4. Switch to **"Tasks" mode**
5. Assign Claude a task

## Example Use Cases

### File Organization
```
"Sort all the PDFs in my Downloads folder by date and move them to appropriate subfolders"
```

### Data Compilation
```
"Create a spreadsheet from all the invoices in this folder with columns for date, vendor, and amount"
```

### Document Creation
```
"Draft a report from these meeting notes with an executive summary"
```

### Research Synthesis
```
"Analyze these research papers and create a summary presentation"
```

## Advanced Features

### Connectors
- Integration with external information sources
- Extend Claude's access beyond local files

### Skills
- Enhanced capabilities for document creation
- Professional presentation generation

### Browser Integration
- Pairs with Claude in Chrome extension
- Web-based task automation

## Current Limitations

| Limitation | Description |
|------------|-------------|
| No Project Support | Cannot access Claude Projects |
| No Memory | No cross-session memory |
| No Sharing | Cannot share tasks/outputs |
| macOS Only | Windows support planned |
| App Open | App must stay open during tasks |

## Safety & Control

- **Selective Access**: You choose which folders/connectors Claude can access
- **User Control**: You maintain oversight of all operations
- **Prompt Injection Defense**: Active development for security
- **Destructive Actions**: Claude can perform if instructed (use caution)

## Roadmap

Planned features:
- Windows support
- Cross-device sync
- Enhanced connectors
- Expanded file type support

## Reference Files

See `references/` for:
- **getting-started.md** - Setup and first steps
- **capabilities.md** - Detailed feature documentation
- **use-cases.md** - Example workflows and patterns

## Resources

- [Getting Started Guide](https://support.claude.com/en/articles/13345190-getting-started-with-cowork)
- [Cowork Announcement Blog](https://claude.com/blog/cowork-research-preview)
- [Claude Desktop Download](https://claude.com/download)

---

*Skill generated from official Anthropic documentation. Last updated: January 2026.*

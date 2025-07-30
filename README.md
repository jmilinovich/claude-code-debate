# Claude Code Debate System

A structured debate system powered by Claude Code that facilitates balanced political discussions between Democratic and Republican perspectives, moderated by an impartial agent and concluded with evidence-based analysis.

## Overview

This project uses Claude Code's custom agents and commands to create comprehensive political debates with:
- Balanced representation of both major US political perspectives
- Web-searched facts and citations for all arguments
- Professional moderation to ensure productive discourse
- Evidence-based truth-seeking analysis and conclusions

## Project Structure

```
.
├── .claude/
│   ├── agents/
│   │   ├── democrat.md         # Progressive Democratic perspective agent
│   │   ├── republican.md       # Conservative Republican perspective agent
│   │   ├── moderator.md        # Balanced debate moderator agent
│   │   └── truth-seeker.md     # Evidence-based analysis agent
│   └── commands/
│       └── debate.md           # Main debate orchestration command
├── debates/                    # Stored debate transcripts and summaries
│   └── YYYY-MM-DD-topic-slug/
│       ├── transcript.md       # Full debate transcript with citations
│       └── summary.md          # Executive summary by truth-seeker
└── CLAUDE.md                   # Project instructions for Claude Code
```

## Usage

To start a new debate, use the custom command:

```
/debate [topic]
```

Example:
```
/debate "Should the US implement universal healthcare?"
```

## How It Works

1. **Initiation**: The `/debate` command triggers the moderator agent
2. **Opening Statements**: Both Democrat and Republican agents present their initial positions with web-searched facts
3. **Moderated Exchange**: The moderator facilitates 2-3 rounds of rebuttals and responses
4. **Closing Arguments**: Each side presents final arguments
5. **Analysis**: The truth-seeker agent provides objective, evidence-based analysis
6. **Storage**: Full transcript and executive summary are saved to the debates folder

## Key Features

- **Web Search Integration**: All agents use real-time web search to find current data, statistics, and expert opinions
- **Citation Requirements**: Every factual claim must include a source URL
- **Balanced Moderation**: The moderator ensures equal speaking time and productive discourse
- **Evidence-Based Conclusions**: The truth-seeker agent focuses on empirical evidence rather than partisan talking points
- **Comprehensive Documentation**: All debates are saved with full transcripts and one-page summaries

## Agent Descriptions

### Democrat Agent (`democrat.md`)
Presents well-researched progressive perspectives, focusing on social justice, government intervention for public good, and evidence-based policy solutions.

### Republican Agent (`republican.md`)
Articulates conservative viewpoints emphasizing free markets, individual liberty, constitutional principles, and limited government.

### Moderator Agent (`moderator.md`)
Maintains debate structure, ensures balanced participation, prevents personal attacks, and guides productive discussion.

### Truth-Seeker Agent (`truth-seeker.md`)
Analyzes all arguments presented, evaluates evidence quality, identifies factual claims vs. opinions, and provides objective assessment based on empirical data.

## Debate Output Format

Each debate generates two files:

1. **transcript.md**: Complete debate record including:
   - All arguments from both sides
   - Citations and source URLs
   - Moderator interventions
   - Truth-seeker's detailed analysis

2. **summary.md**: One-page executive summary containing:
   - Key arguments from each side
   - Most compelling evidence presented
   - Truth-seeker's main findings
   - Evidence-based conclusions

## Requirements

- Claude Code CLI installed and configured
- Active internet connection for web search functionality
- Git for version control (optional)

## Contributing

This is a Claude Code project designed to demonstrate balanced political discourse. Contributions that enhance objectivity, improve citation quality, or expand debate capabilities are welcome.

## License

This project is open source and available for educational and research purposes.
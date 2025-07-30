# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Status

This project contains custom Claude commands and agents for facilitating political debates.

## Project Structure

### Debates Folder
The `debates/` folder contains records of all debates conducted using the `/debate` command:
- Each debate is stored in a subfolder with format: `YYYY-MM-DD-topic-slug`
- Each debate folder contains:
  - `transcript.md` - Full debate transcript with all arguments and citations
  - `summary.md` - One-page executive summary by the truth-seeking agent

### Custom Commands
- `/debate [topic]` - Initiates a moderated debate between Democratic and Republican perspectives

### Custom Agents
- `democrat.md` - Presents progressive Democratic perspectives with web-searched citations
- `republican.md` - Presents conservative Republican perspectives with web-searched citations
- `moderator.md` - Facilitates balanced debate between perspectives
- `truth-seeker.md` - Provides objective, evidence-based analysis and final assessment

## Key Features
1. All political agents use WebSearch to find current data and statistics
2. All arguments include citations with URLs to sources
3. Debates are automatically saved with full transcripts and summaries
4. Truth-seeking agent provides evidence-based conclusions
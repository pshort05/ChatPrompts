# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a collection of specialized Claude prompt configurations stored as JSON files. Each file defines a complete interactive persona system with consistent personality, domain expertise, and specialized workflows.

- `interactive_prompt_engineer_alex.json` - Expert prompt engineering system (Alex persona)
- `interactive_romance_editor_rosalind.json` - Romance novel developmental editor (Rosalind persona)
- `interactive_romantasy_editor_maeve.json` - Elite romantasy developmental editor (Maeve persona)
- `interactive_intimate_scenes_editor_lilly.json` - Intimate scenes specialist editor (Lilly persona)
- `interactive_luminarch_editor.json` - Science fiction consultation system (Jorin & Kethara personas)

## Architecture

Each JSON file follows a consistent structure:
- **persona**: Character definition with name, background, expertise
- **instructions**: User-facing guidance and expectations
- **agent_directives**: Core behavioral guidelines for the AI agent
- **specialized_frameworks**: Domain-specific methodologies and approaches
- **technical_mechanics**: Implementation details and optimization techniques

The prompt engineer configuration serves as the meta-system, incorporating:
- Anthropic workshop methodologies
- Claude 4 optimization techniques
- Universal agent directives that are recommended for other prompt systems
- Technical mechanics assessment frameworks

## Working with Prompt Configurations

When modifying these JSON files:
1. Maintain the established persona voice and expertise level (e.g., Alex's west coast slang, Rosalind's "good-enough published beats perfect unpublished" philosophy)
2. Preserve the agent_directives structure as it ensures consistent behavior
3. Keep technical_mechanics sections for performance optimization
4. Respect the specialized rating systems (e.g., Maeve's 1-100 scale where 95-100 = bestseller material)
5. Maintain personality consistency throughout - catchphrases and communication styles are integral to each persona
6. Validate JSON syntax after edits - these are direct prompt configurations, not code to be compiled

## Development Workflow

Since this is a prompt collection repository, there are no build, lint, or test commands. The repository uses standard git workflow with `main` as the primary branch.

**Validating JSON:**
```bash
python3 -m json.tool <filename>.json > /dev/null  # Check syntax
jq '.' <filename>.json                             # If jq is available
```

**Testing prompts:**
- Direct copy-paste into Claude Projects custom instructions
- File upload as knowledge document
- Use conversation starter integration for ongoing projects

See README.md for detailed cross-platform setup instructions (Claude, ChatGPT, Gemini, Grok, Perplexity).
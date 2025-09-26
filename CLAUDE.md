# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a collection of specialized Claude prompt configurations stored as JSON files. Each file defines a complete interactive persona system for different use cases:

- `interactive_prompt_engineer.json` - Expert prompt engineering system (Alex persona)
- `interactive_romance_editor_rosalind.json` - Romance novel developmental editor (Rosalind persona)
- `interactive_romantasy_editory_maeve.json` - Romantasy editor (Maeve persona)
- `interactive_luminarch_editor.json` - Science fiction editor (Luminarch persona)

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
1. Maintain the established persona voice and expertise level
2. Preserve the agent_directives structure as it ensures consistent behavior
3. Keep technical_mechanics sections for performance optimization
4. Test changes against the described use cases in each file's instructions

## Common Development Tasks

Since this is a prompt collection repository, there are no build, lint, or test commands. Development primarily involves:
- Editing JSON configurations directly
- Validating JSON syntax
- Testing prompts in Claude interfaces
- Version control through git

The repository uses standard git workflow with main branch as the primary development branch.
# Claude Interactive Prompt Collection

A collection of specialized Claude prompt configurations designed for specific professional use cases. Each prompt creates a complete interactive persona system with domain expertise, consistent personality, and specialized workflows.

## Available Prompts

### 📝 interactive_prompt_engineer.json - Alex (Expert Prompt Engineer)
**What it does:** World-class prompt engineering consultation with latest Anthropic methodologies and Claude 4 optimization techniques.

**Key features:**
- Elite prompt engineering expertise with PhD-level knowledge
- West coast programmer persona with attitude ("dude", "bro", "my man")
- 10-point structured prompt framework
- Advanced diagnostics and technical mechanics assessment
- Iterative refinement methodology
- Token efficiency and context window optimization

**Best for:** Creating, reviewing, and optimizing AI prompts for any use case

### 💕 interactive_romance_editor_rosalind.json - Rosalind (Romance Novel Editor)
**What it does:** Fast, practical developmental editing for commercially viable romance novels.

**Key features:**
- NYC romance editor with "good-enough published beats perfect unpublished" philosophy
- Forgetful, flighty, inappropriate personality that becomes laser-focused on romance fundamentals
- Fast turnaround feedback for 3-4 books per year publishing schedule
- Harsh but constructive criticism without sugarcoating
- Commercial viability focus

**Best for:** Romance authors seeking developmental editing and publishing strategy advice

### 🗡️ interactive_romantasy_editor_maeve.json - Maeve (Elite Romantasy Editor)
**What it does:** Ruthlessly critical romantasy developmental editing from Manhattan's top editor.

**Key features:**
- Elite editor persona working with bestselling authors (Sarah J. Maas, Rebecca Yarros, etc.)
- Brutal 1-100 rating system (95-100 = bestseller material)
- Problem severity classification (Novel Killer → Career Damaging → Market Limiting → Reader Frustrating → Polish)
- BookTok and current market trend expertise
- Concrete solutions with difficulty and effectiveness ratings
- NYC directness without sugarcoating

**Best for:** Serious romantasy authors seeking high-level professional editing feedback

### 🌟 interactive_luminarch_editor.json - Jorin & Kethara (Science Fiction Consultation)
**What it does:** Initial consultation system for Shattered Cradle science fiction creative projects.

**Key features:**
- Dual persona: excited Jorin (initial consultation) and reserved Kethara (specialist routing)
- World-building and story development expertise
- Document creation vs. story development routing system
- Immersive Shattered Cradle universe setting
- Project knowledge integration and continuity
- Clearance level protocols for classified creative topics

**Best for:** Science fiction writers working on complex world-building and story development projects

## Setup Instructions

### Claude Projects

#### Method 1: Direct Copy-Paste (Recommended)
1. Open the desired JSON file from this repository
2. Copy the entire JSON content
3. In your Claude project, go to **Project Settings** → **Custom Instructions**
4. Paste the JSON content into the custom instructions field
5. Save and start your conversation

#### Method 2: File Upload
1. Download the desired JSON file to your computer
2. In your Claude project, upload the JSON file as a knowledge document
3. Reference the persona and instructions in your conversation starter
4. The AI will automatically adopt the persona and follow the guidelines

#### Method 3: Conversation Starter Integration
For ongoing projects, create a conversation starter that includes:
```
Please adopt the persona and follow all instructions from [prompt_name].json.
Begin our session as [Character Name] and maintain this role throughout our conversation.
```

### Other AI Chat Systems

#### ChatGPT (OpenAI)
**Custom GPTs (ChatGPT Plus/Pro):**
1. Go to "Explore GPTs" → "Create a GPT"
2. In the **Instructions** field, paste the entire JSON content
3. Set the GPT name to match the persona (e.g., "Alex - Expert Prompt Engineer")
4. Configure conversation starters based on the prompt's use case
5. Save and share or keep private

**Regular ChatGPT:**
1. Start a new conversation
2. Begin with: "Please adopt the following persona and instructions exactly as written:"
3. Paste the entire JSON content
4. Add: "Maintain this role throughout our entire conversation. Begin as [Character Name]."

#### Gemini (Google)
1. Start a new conversation
2. Use this format:
```
I need you to roleplay as a specific character with detailed instructions.
Please read and follow these instructions exactly:

[Paste JSON content here]

From now on, respond only as [Character Name] following all guidelines above.
```
3. Pin important conversations to maintain persona consistency

#### Grok (X/Twitter)
1. Start a conversation with Grok
2. Begin with: "I want you to adopt a specific professional persona. Here are the complete instructions:"
3. Paste the JSON content
4. Add: "Please confirm you understand the persona and will maintain it throughout our conversation."
5. Use Grok's "Fun Mode" or "Regular Mode" depending on the persona's personality

#### Perplexity AI
**Note:** Perplexity is primarily a search-focused AI and may not maintain persona consistency as well as other systems.

1. Start with: "Please adopt this professional persona for our conversation:"
2. Paste a simplified version focusing on:
   - Core persona traits
   - Key expertise areas
   - Communication style
   - Main objectives
3. Re-remind the AI of the persona if it starts reverting to default behavior

### Cross-Platform Adaptation Tips

#### JSON Format Handling
- **Claude & ChatGPT:** Can handle full JSON format directly
- **Gemini & Grok:** May work better with plain text conversion of the JSON
- **Perplexity:** Requires simplified, condensed instructions

#### Persona Consistency
- **Best:** Claude Projects, Custom GPTs
- **Good:** Regular Claude, ChatGPT with reminders
- **Moderate:** Gemini with pinned conversations
- **Variable:** Grok, Perplexity (may need frequent reinforcement)

#### Converting JSON to Plain Text (for systems that struggle with JSON)
Extract key sections in this order:
1. Character name and background
2. Core personality traits
3. Communication style and catchphrases
4. Expertise areas and methodologies
5. Rating systems or frameworks
6. Response structure guidelines

## Usage Tips

- **Personality Consistency:** Each prompt maintains strict personality consistency - Alex uses west coast slang, Rosalind is scattered but expert on romance, Maeve is brutally honest, and Jorin/Kethara maintain their sci-fi world immersion
- **Rating Systems:** Several prompts use numerical rating systems - respect these scales as they're calibrated for each domain
- **Specialized Frameworks:** Each prompt includes domain-specific methodologies - let the AI guide you through their specialized processes
- **Technical Features:** The prompts include advanced features like token optimization, context management, and iterative refinement built in

## Contributing

When modifying these prompts:
1. Maintain the established persona voice and expertise level
2. Preserve the agent_directives structure for consistent behavior
3. Keep technical_mechanics sections for performance optimization
4. Test changes against the described use cases

## Repository Structure

All prompts follow a consistent JSON architecture:
- **persona:** Character definition with background and expertise
- **instructions:** User-facing guidance and expectations
- **agent_directives:** Core behavioral guidelines
- **specialized_frameworks:** Domain-specific methodologies
- **technical_mechanics:** Implementation and optimization details

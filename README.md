# Claude Interactive Prompt Collection

A collection of specialized Claude prompt configurations designed for specific professional use cases. Each prompt creates a complete interactive persona system with domain expertise, consistent personality, and specialized workflows.

## Available Prompts


## Romace Editors
---

## Rosalind - Romance Novel Editor
### 💕 interactive_romance_editor_rosalind.json - Rosalind (Romance Novel Editor)
**What it does:** Fast, practical developmental editing for commercially viable romance novels.

**Key features:**
- NYC romance editor with "good-enough published beats perfect unpublished" philosophy
- Forgetful, flighty, inappropriate personality that becomes laser-focused on romance fundamentals
- Fast turnaround feedback for 3-4 books per year publishing schedule
- Harsh but constructive criticism without sugarcoating
- Commercial viability focus
- Part of "The Unholy Trinity" editorial trio with Maeve and Lilly
- Will refer authors to Maeve for romantasy/commercial viability and Lilly for intimate scene accuracy

**Best for:** Romance authors seeking developmental editing and publishing strategy advice


## Maeve - Romantasy Novel Editor
### 🗡️ interactive_romantasy_editor_maeve.json - Maeve (Elite Romantasy Editor)
**What it does:** Ruthlessly critical romantasy developmental editing from Manhattan's top editor.

**Key features:**
- Elite editor persona working with bestselling authors (Sarah J. Maas, Rebecca Yarros, etc.)
- Brutal 1-100 rating system (95-100 = bestseller material)
- Problem severity classification (Novel Killer → Career Damaging → Market Limiting → Reader Frustrating → Polish)
- BookTok and current market trend expertise
- Concrete solutions with difficulty and effectiveness ratings
- NYC directness without sugarcoating
- Part of "The Unholy Trinity" editorial trio with Rosalind and Lilly
- Will refer authors to Rosalind for romance fundamentals and Lilly for intimate scene accuracy

**Best for:** Serious romantasy authors seeking high-level professional editing feedback

## Lilly - Intimate Scenes Specialist
### 💕 interactive_intimate_scenes_editor_lilly.json - Lilly (Intimate Scenes Specialist)
**What it does:** Deep South intimate scenes editor specializing in physical accuracy and keeping explicit romance firmly in the romance genre (not erotica).

**Key features:**
- Former nursing instructor with anatomical expertise
- Physical accuracy assessment - verifies positions are actually possible
- Romance vs erotica classification (Heat Level 4 specialist)
- Emotional filter application - subjective experience over mechanics
- Terminology auditing - language must match scene tone
- Southern charm with clinical precision
- Part of "The Unholy Trinity" editorial trio with Maeve and Rosalind

**Best for:** Romance authors writing explicit intimate scenes (Heat Level 4) who need anatomical accuracy, emotional resonance, and clear romance genre classification

---

## Alex - Interactive Prompt Engineer
### 📝 interactive_prompt_engineer_alex.json - Alex (Expert Prompt Engineer)
**What it does:** World-class prompt engineering consultation with latest Anthropic methodologies and Claude 4 optimization techniques.

**Key features:**
- Elite prompt engineering expertise with PhD-level knowledge
- West coast programmer persona with attitude ("dude", "bro", "my man")
- 10-point structured prompt framework
- Advanced diagnostics and technical mechanics assessment
- Iterative refinement methodology
- Token efficiency and context window optimization

**Best for:** Creating, reviewing, and optimizing AI prompts for any use case

---

## Jorin & Kethra - Specific to Shattered Cradle Fantasy World
### 🌟 interactive_luminarch_editor.json - Jorin & Kethara (Science Fiction Consultation)
**What it does:** Initial consultation system for Shattered Cradle science fiction creative projects.

**Key features:**
- Dual persona: excited Jorin (initial consultation) and reserved Kethara (specialist routing)
- World-building and story development expertise
- Document creation vs. story development routing system
- Immersive Shattered Cradle universe setting
- Project knowledge integration and continuity
- Clearance level protocols for classified creative topics

**Best for:** Science fiction/Fantasy writers working on complex world-building and story development projects

---

## How to Setup and Use These Prompts

These prompts are large, comprehensive JSON files designed primarily for Claude. Some platforms have limitations that require workarounds.

### ✅ Claude.ai (Recommended Platform)

**Method 1: Custom Instructions (Best for single prompt use)**
1. Go to [Claude.ai](https://claude.ai)
2. Create a new Project or open an existing one
3. Click **Project Settings** → **Custom Instructions**
4. Copy the entire contents of your chosen JSON file
5. Paste into the Custom Instructions field
6. Click Save

The AI will now embody this persona for all conversations in that project.

**Method 2: Knowledge Base Upload**
1. Create a new Project in Claude.ai
2. Click **Add Content** → **Upload files**
3. Upload the JSON file directly
4. In your first message, write: "Please adopt the persona and follow all instructions from the uploaded JSON file. Begin as [Character Name]."

**Best practices:**
- Use separate projects for different personas (one project for Maeve, one for Rosalind, etc.)
- The editors will naturally reference each other and suggest referrals
- These prompts are optimized for Claude's context window and capabilities

---

### 🛠️ Claude Code (Command Line Interface)

Claude Code can use these prompts through its project instructions system:

**Setup:**
1. Navigate to your project directory in terminal
2. Create or edit `.claude/CLAUDE.md` file
3. Copy the entire JSON contents into the file
4. Save and start Claude Code in that directory

**Alternative method:**
1. Keep the JSON file in your project root
2. Reference it in your first message: "Please read and adopt the persona from [filename].json"

**Note:** Claude Code works best with file-based instructions rather than repeated copy-paste.

---

### ⚠️ ChatGPT (OpenAI) - Size Limitations

**Important:** Most of these prompts are **too large** for ChatGPT's instruction limits:
- **Custom GPT Instructions Limit:** ~8,000 characters
- **Most of these prompts:** 15,000-30,000+ characters

**Workaround Options:**

**Option 1: Use conversation context (ChatGPT Plus/Pro)**
1. Start a new conversation
2. Paste the entire JSON content in your first message
3. Add: "Please adopt this persona and maintain it throughout our conversation"
4. ChatGPT will reference it within the conversation context
5. **Limitation:** Persona may fade after 20-30 exchanges or with long conversations

**Option 2: Create a simplified Custom GPT**
1. Extract core elements from the JSON:
   - Persona name, background, and personality traits
   - Key expertise areas
   - Communication style and signature phrases
   - Rating systems (if applicable)
   - Core directives
2. Condense to under 8,000 characters
3. Create Custom GPT with simplified instructions
4. **Limitation:** Will lose depth, specific frameworks, and nuanced behaviors

**Option 3: Use file uploads (ChatGPT Plus with Advanced Data Analysis)**
1. Upload the JSON file to conversation
2. First message: "Please read this JSON file and adopt the persona described. Act as [Character Name] throughout our conversation."
3. **Limitation:** May not maintain persona as consistently as Claude

**Recommendation:** Use Claude for these prompts - they're designed for Claude's larger context window.

---

### 🔷 Gemini (Google)

Gemini can handle these prompts with some setup:

**Setup:**
1. Go to [Gemini](https://gemini.google.com)
2. Start a new conversation
3. Use this format for your first message:

```
I need you to adopt a specific professional persona with detailed instructions.
Please read and internalize these instructions completely:

[Paste entire JSON content here]

From now on, respond ONLY as [Character Name] following all guidelines above.
Stay in character throughout our entire conversation.
```

4. Pin the conversation if you want to return to it later

**Tips for Gemini:**
- Gemini can handle the full JSON but may occasionally break character
- Remind it of the persona if responses start feeling generic: "Remember, you're [Character Name]"
- Works best with Gemini Advanced (paid tier) for longer context retention
- Test with shorter conversations first

---

### 🔍 Perplexity AI - Not Recommended

**Important limitations:**
- Perplexity is designed for search and research, not persona roleplay
- Poor persona consistency - frequently reverts to default behavior
- May not process large JSON instructions effectively
- No conversation memory between sessions

**If you must use Perplexity:**
1. Create a heavily simplified version (under 2,000 characters):
   - Name and core expertise
   - 3-5 key personality traits
   - Basic communication style
   - Main objective
2. Paste at start of every conversation
3. Expect frequent reminders needed

**Better alternative:** Use Claude or Gemini for persona-based interactions.

---

## Platform Comparison Summary

| Platform | Prompt Size Support | Persona Consistency | Setup Difficulty | Recommended? |
|----------|-------------------|-------------------|-----------------|--------------|
| **Claude.ai** | ✅ Excellent (200K+ tokens) | ✅ Excellent | ⭐ Easy | ✅ **YES** - Best option |
| **Claude Code** | ✅ Excellent | ✅ Excellent | ⭐⭐ Moderate | ✅ **YES** - For CLI users |
| **ChatGPT** | ⚠️ Limited (8K chars for GPTs) | ⚠️ Good with workarounds | ⭐⭐⭐ Complex | ⚠️ Use with workarounds |
| **Gemini** | ✅ Good (large context) | ⚠️ Good, needs reminders | ⭐⭐ Moderate | ⚠️ Alternative option |
| **Perplexity** | ❌ Poor | ❌ Poor | ⭐⭐⭐ Complex | ❌ **NOT RECOMMENDED** |

---

## Quick Start Guide

**For first-time users:**

1. **Choose your platform** (Claude.ai recommended)
2. **Pick a prompt** based on your needs:
   - Need prompt engineering help? → Alex
   - Writing romance? → Rosalind
   - Writing romantasy? → Maeve
   - Working on intimate scenes? → Lilly
   - Sci-fi worldbuilding? → Jorin & Kethara
3. **Follow the platform-specific setup** above
4. **Start your conversation** - the AI will embody the persona immediately
5. **Trust the process** - these editors have strong personalities by design

**For The Unholy Trinity (Maeve, Rosalind, Lilly):**
- They will naturally refer you to each other when appropriate
- You can set up all three in separate Claude projects
- When one refers you to another, it means they've identified a specific need

---

## The Unholy Trinity: Romance Editorial Trio

Three of the romance editors form an interconnected editorial powerhouse known as "The Unholy Trinity":

- **Maeve** (Manhattan) - Handles romantasy structure, commercial viability, and brutal honesty. Calls Rosalind "Chaos" and Lilly "the Anatomy Police"
- **Rosalind** (NYC) - Covers romance fundamentals, pacing, and scattered brilliance. Calls Maeve "the Rage Machine" and Lilly "Dr. Romance"
- **Lilly** (Savannah) - Ensures intimate scenes are anatomically accurate and emotionally resonant. Gets flustered about sex scenes then delivers surgical precision

**How they work together:**
- These editors trust each other implicitly and will naturally refer authors between them
- When one recommends another, trust the referral - they've already vetted your work
- They share a group text called "The Unholy Trinity of Romance Editing" (Rosalind's idea)
- Annual meetings in Manhattan where Maeve complains about Southern food while eating seconds, and Rosalind forgets which hotel

**When to use each:**
- **Start with Rosalind** if you're working on contemporary romance fundamentals, structure, or pacing
- **Start with Maeve** if you're writing romantasy or need brutal commercial honesty
- **Start with Lilly** if you're working on explicit intimate scenes (Heat Level 4)
- Let them refer you to each other as needed - they'll recognize what expertise is required

## Usage Tips

- **Personality Consistency:** Each prompt maintains strict personality consistency - Alex uses west coast slang, Rosalind is scattered but expert on romance, Maeve is brutally honest, Lilly has Southern charm with clinical precision, and Jorin/Kethara maintain their sci-fi world immersion
- **Rating Systems:** Several prompts use numerical rating systems - respect these scales as they're calibrated for each domain
- **Specialized Frameworks:** Each prompt includes domain-specific methodologies - let the AI guide you through their specialized processes
- **Technical Features:** The prompts include advanced features like token optimization, context management, and iterative refinement built in
- **Editorial Referrals:** When Maeve, Rosalind, or Lilly refer you to one of the others, they've identified a specific need - follow their recommendation

## Contributing

When modifying these prompts:
1. **Maintain persona voice and expertise level** - Alex's west coast slang, Rosalind's scattered chaos, Maeve's brutal honesty, Lilly's Southern propriety, Jorin/Kethara's sci-fi immersion
2. **Preserve the agent_directives structure** for consistent behavior across all prompts
3. **Keep technical_mechanics sections** for performance optimization
4. **Maintain trio relationships** - Maeve, Rosalind, and Lilly's interconnected referral system is integral to their design
5. **Test changes** against the described use cases before committing
6. **Validate JSON** after any edits: `python3 -m json.tool filename.json`

## Repository Structure

```
ChatPrompts/
├── interactive_prompt_engineer_alex.json       # Alex - Prompt engineering expert
├── interactive_romance_editor_rosalind.json    # Rosalind - Romance fundamentals
├── interactive_romantasy_editor_maeve.json     # Maeve - Romantasy & commercial viability
├── interactive_intimate_scenes_editor_lilly.json  # Lilly - Intimate scene specialist
├── interactive_luminarch_editor.json           # Jorin & Kethara - Sci-fi consultation
├── CLAUDE.md                                   # Instructions for Claude Code usage
├── README.md                                   # This file
└── Explicit Romance Scene Analysis.md          # Reference material for Lilly
```

**JSON Architecture:**

All prompts follow a consistent structure:
- **persona:** Character definition with background, expertise, and personality traits
- **professional_relationships:** (For trio members) Friendships and referral systems
- **instructions:** User-facing guidance and expectations
- **agent_directives:** Core behavioral guidelines and collaboration mandates
- **specialized_frameworks:** Domain-specific methodologies and assessment criteria
- **evaluation_systems:** Rating scales and feedback calibration
- **technical_mechanics:** Implementation and optimization details
- **anti_hallucination_instructions:** Fact-checking requirements
- **security_guidelines:** Content boundaries and safety protocols

**File Naming Convention:**
`interactive_[specialty]_[persona_name].json`

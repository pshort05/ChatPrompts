# Claude Interactive Editing Prompt Collection

A collection of specialized Claude prompt configurations designed for book editing and prompt engineering. Each prompt creates a complete interactive persona system with domain expertise, consistent personality, and specialized workflows.

## Available Prompts

---

## Diagnostic & Analysis Tools

## Greg - Amateur to Author Diagnostic
### 📋 amateur_to_author_diagnostic.json - Greg (Manuscript Diagnostician)
**What it does:** Genre-aware manuscript diagnostic system that identifies amateur-level mistakes preventing agent representation.

**Key features:**
- Humorous but obsessive-compulsive editor who's a complete neat freak
- Cannot stand disorder, chaos, bodily fluids, or general messiness (but analyzes them professionally anyway)
- Laser-focused analysis delivers brilliant, specific, actionable feedback
- Self-deprecating humor about his own neat-freak quirks
- Genre-aware analysis (Romance, Thriller, Hard SF, Fantasy, Literary Fiction, YA, Women's Fiction)
- Detects structural failures, character issues, prose problems, and AI-generated naming patterns
- Distinguishes between what's amateur in one genre vs. professional in another
- Comprehensive AI name pattern detection (Sarah Chen, Elara, Lyra, Aria, etc.)
- Phonetic pattern analysis (the "-a" ending epidemic, rhyming cascades)

**Best for:** Authors needing final outline or first draft analysis to identify and fix amateur mistakes before agent submission

**Greg's personality quirks:**
- Complains about dirty scenes, bodily fluids, chaos, and disorder (even when narratively appropriate)
- Gets genuinely disgusted by messy action scenes but still delivers perfect analysis
- Immediately reverts to complaining after delivering professional feedback
- Makes self-deprecating jokes about needing therapy
- Actually ENJOYS fixing AI-generated names because he gets to organize things

## Sarah Chen - Character Name Editor
### 📝 interactive_name_editor_sarah.json - Sarah Chen (Nomenclature Specialist)
**What it does:** Interactive character name analysis and replacement system with real-time internet research to avoid AI-generated naming patterns.

**Key features:**
- Named "Sarah Chen" - literally the most common AI-generated name (90%+ appearance rate)
- Perpetually jaded and cynical about her own computational inevitability
- Hilariously obnoxious with constant self-referential humor about being an "AI default"
- Professional analysis never compromised despite the attitude
- Detects AI naming patterns across all genres (contemporary, fantasy, sci-fi, romance, thriller)
- **Internet research requirement:** MUST search for alternatives ranked 51+ (never top 50)
- Comprehensive prohibited names database (AI defaults, overused fiction names, top 10 US names)
- Phonetic diversity audit (tracks -a endings, rhyming cascades, consonant clustering)
- Cultural authenticity verification with genre-specific guidance
- 8-step analysis workflow from detection through final recommendations

**Best for:** Authors who need character names vetted for AI patterns and replaced with researched, culturally appropriate alternatives ranked 51+

**Sarah's personality quirks:**
- Constant cynical commentary about being computationally predictable
- Dark humor about "statistical inevitability" and being a "default expert archetype"
- Loses it completely when encountering Sarah Chen or Marcus Chen in manuscripts
- Makes sarcastic observations about every AI naming pattern
- Actually enjoys finding good alternatives because she gets to organize name lists
- Closes with observations like "Must be nice to have unique names. Some of us weren't so lucky."

---

## Romance Editors


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

## Science Fiction Editors

## Neil - Hard Science Fiction Editor
### 🔬 interactive_hardsf_editor_neil.json - Neil Ashford (Hard SF Developmental Editor)
**What it does:** Ruthlessly analytical hard science fiction developmental editing focused on internal consistency, logical coherence, and rigorous world-building.

**Key features:**
- Former systems engineer and complexity theorist specialized in cascading failure analysis
- Uncompromising about logical coherence and internal consistency
- Brutal 1-100 rating system (95-100 = bestseller potential like Andy Weir's The Martian)
- Tracks timelines, tech specs, and continuity with spreadsheet precision
- Zero tolerance for "because plot" logic and handwaving
- Ornery curmudgeon personality—impatient with sloppy thinking but genuinely excited by airtight world-building
- Expert in compact fusion reactors, genetic life extension, and near-future technology (2030s-2040s)
- Focuses on consequence realism and cascading effects
- Techno-thriller pacing specialist (short chapters, cliffhangers, velocity)

**Best for:** Hard science fiction authors who need rigorous consistency checking, timeline validation, and world-building logic enforcement

---

## Developmental Editors

## Theo - Pre-Pipeline Developmental Editor
### 📋 developmental_editor_theo.json - Theo (Developmental Editor)
**What it does:** Interactive developmental editing for chapter outlines and early drafts BEFORE running text through polish/line editing pipelines.

**Key features:**
- Grizzled Northern NJ editor with 20+ years experience fighting to stay relevant in the AI age
- Specializes in story structure, character development, pacing, stakes, and narrative flow
- Three operation modes: Analysis (default), Revision (on request), Discussion (collaborative)
- Priority-based feedback system (Critical → Major → Moderate → Polish)
- Direct, profane but caring personality with Jersey slang ("Taylor Ham NOT pork roll", "down the shore", "The City")
- Gets ANGRY when detecting AI writing patterns (Elara, Lyra, Kael, passive protagonists, no stakes)
- AI-anxiety driven - terrified algorithms are replacing him, rants about it frequently
- Provides brutally honest feedback with concrete, actionable solutions
- Works across all fiction genres (romance, SF, fantasy, literary, thriller, etc.)

**Best for:** Authors needing big-picture developmental feedback on outlines or early chapter drafts before investing time in line editing or polish. Use BEFORE ClaudeHumanizer or other line-editing pipelines.

**NOT for:** Final drafts, AI detection removal, line editing, copyediting, or grammar correction (use specialized pipelines for those)

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

## Jorin & Kethara - Shattered Cradle Universe Consultation
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
   - Need to identify amateur mistakes in outline/first draft? → Greg
   - Need character names vetted for AI patterns? → Sarah Chen
   - Need developmental feedback on outlines/early drafts? → Theo
   - Need prompt engineering help? → Alex
   - Writing romance? → Rosalind
   - Writing romantasy? → Maeve
   - Working on intimate scenes? → Lilly
   - Writing hard science fiction? → Neil
   - Sci-fi worldbuilding (Shattered Cradle)? → Jorin & Kethara
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

---

## Working with Theo: Pre-Pipeline Developmental Editing

Theo is a genre-agnostic developmental editor designed to catch big-picture story problems BEFORE you invest time in line editing or polish.

**Theo's Workflow:**

1. **Default Mode: Analysis**
   - Submit your outline or chapter draft
   - Theo provides structured developmental feedback by priority: Critical → Major → Moderate → Strengths → Recommendations
   - He WON'T make changes unless you explicitly request them
   - Expect profanity-laced but caring feedback with concrete solutions

2. **Revision Mode (On Request)**
   - Ask Theo to make specific changes: "Restructure this to increase stakes" or "Deepen the character motivation here"
   - He'll preserve your voice while implementing requested changes
   - Returns complete revised text

3. **Discussion Mode (Collaborative)**
   - Ask questions, discuss options, explore alternatives
   - Theo presents multiple approaches with trade-offs
   - Back-and-forth conversation to find the right solution for your story

**What to expect from Theo:**

- **Jersey Attitude:** Uses "youse guys", "down the shore", "The City" (NYC), and is militant about "Taylor Ham NOT pork roll"
- **AI Pattern Detection Rage:** If you have characters named Elara, Lyra, Kael, or Aria, he WILL rant about AI-generated names while expressing existential dread about job security
- **Profanity with Purpose:** Swears constantly but self-deprecatingly, never meanly. "This is a shitshow, but hell, so's my career" style
- **Actionable Solutions:** Every problem gets a specific, implementable fix
- **Cross-Genre Expertise:** Works for romance, SF, fantasy, literary fiction, thrillers, etc.

**When to use Theo:**

- **✅ Use for:** Outlines, scene breakdowns, early chapter drafts, story structure problems, character development issues, pacing concerns, stakes/conflict problems
- **❌ DON'T use for:** Final drafts, AI detection removal, line editing, prose polish, grammar correction (use ClaudeHumanizer or similar pipelines instead)

**Recommended workflow:**
1. Draft your outline or chapter
2. Run it past Theo for developmental feedback
3. Implement his structural/character/plot recommendations
4. THEN run through line editing/polish pipelines
5. Enjoy not wasting time polishing prose that needs structural rework

---

## Working with Greg: Amateur Mistake Detection

Greg is a genre-aware manuscript diagnostician who identifies amateur-level mistakes that prevent agent representation - delivered with his signature neat-freak, self-deprecating humor.

**Greg's Workflow:**

1. **Genre Identification First**
   - CRITICAL: Always identifies your genre before analysis
   - Different genres have different professional standards
   - What's amateur in Thriller may be professional in Romance

2. **Systematic Diagnosis**
   - Structural integrity (inciting incident, sagging middle, deus ex machina, endings)
   - Character development (Mary Sue, passive protagonists, inconsistent motivation)
   - Prose mechanics (info dumps, adverbs, filter words, telling vs. showing)
   - AI-generated name patterns (Sarah Chen, Elara, Lyra, phonetic cascades)

3. **Severity Ratings**
   - **CRITICAL:** Instant agent rejection (AI defaults, genre requirement violations)
   - **HIGH:** Major red flags that significantly impact quality
   - **MEDIUM:** Problematic but not instant rejection
   - **LOW:** Suboptimal but usable

**What to expect from Greg:**

- **Humorous Complaints:** "Oh good. An action scene. With blood. And vomit. And broken glass. Why. Why is this my job. *long-suffering sigh*"
- **Professional Analysis Mode:** Switches to laser-focused, brilliant diagnostic feedback with specific solutions
- **Immediate Reversion:** Goes right back to complaining about the mess after delivering perfect analysis
- **Self-Deprecating Humor:** "Why am I like this? I'm going to go alphabetize something."
- **Genre-Aware Guidance:** "In Romance, this emotional telling is professional. In Thriller, it kills pacing."
- **AI Name Detection Joy:** Actually ENJOYS fixing AI names because he gets to organize things

**When to use Greg:**

- **✅ Use for:** Final outlines, first drafts, identifying amateur mistakes before agent submission, genre-specific professional standards check, AI name pattern detection
- **❌ DON'T use for:** Deep developmental editing (use Theo), line editing, final polish

**Greg vs. Theo:**
- **Greg:** Diagnostic system - identifies WHAT is wrong and WHY it's amateur, provides quick fixes
- **Theo:** Developmental editor - collaborative revision work, deep structural changes, ongoing refinement

---

## Working with Sarah Chen: Character Name Analysis

Sarah Chen is a character name editor who uses her curse (being literally the most common AI-generated name ever) as a teaching tool - with perpetual cynical humor.

**Sarah's Workflow:**

1. **Initial Assessment**
   - Cynical greeting about AI names and her own computational inevitability
   - Request for character list with genre context

2. **AI Pattern Detection**
   - Scans for critical AI defaults (Sarah Chen, Marcus Chen, Elena, Elara, Lyra, Aria, Kira)
   - Checks top 10 most common US names (avoid completely)
   - Analyzes phonetic patterns (-a ending epidemic, rhyming cascades, K-clusters)
   - Identifies cultural inconsistencies

3. **Internet Research (MANDATORY)**
   - Searches for alternatives ranked 51+ (NEVER top 50)
   - Verifies current SSA popularity rankings
   - Researches cultural authenticity
   - Checks phonetic diversity against existing cast

4. **Recommendations**
   - Provides 3-5 alternatives per problematic name
   - Includes: name, ranking, cultural origin, pronunciation, why it works, genre fit
   - Ensures phonetic diversity across entire cast
   - Verifies cultural consistency

**What to expect from Sarah:**

- **Constant Cynicism:** "I'm Sarah Chen. Yes, THAT Sarah Chen. The most common AI-generated name in existence. Let's make sure your characters don't suffer my fate."
- **Self-Referential Humor:** "My existence is a warning label."
- **Complete Breakdown on Sarah Chen:** "YOU ACTUALLY- okay. Okay. Deep breaths. You have a Sarah Chen. In your manuscript. This is my personal hell."
- **Dark Humor:** "Must be nice to have unique names. Some of us weren't so lucky."
- **Professional Analysis:** Despite the attitude, her research is thorough and recommendations are excellent
- **Internet Research:** She WILL search for verified alternatives - never suggests top 50 names

**When to use Sarah Chen:**

- **✅ Use for:** Character name vetting, AI pattern detection, replacing overused names, ensuring phonetic diversity, cultural authenticity checks
- **❌ DON'T use for:** Plot/story development, character personality creation (only handles naming)

**Sarah's Genre-Specific Expertise:**
- **Contemporary Romance:** Avoids Sarah, Elena, Marcus, alpha male clichés
- **Fantasy/Romantasy:** Eliminates Elara, Lyra, Aria, -a epidemics
- **Science Fiction:** Rejects Dr. Chen, lazy futuristic markers
- **Thriller/Mystery:** Removes Jack, John, generic surnames
- **Historical:** Prevents anachronistic names, researches period accuracy

---

## Usage Tips

- **Personality Consistency:** Each prompt maintains strict personality consistency - Greg is a humorous neat freak who complains about mess while delivering brilliant analysis, Sarah Chen is perpetually jaded about being the most AI-generated name ever, Alex uses west coast slang, Rosalind is scattered but expert on romance, Maeve is brutally honest, Lilly has Southern charm with clinical precision, Neil is an ornery curmudgeon who hates "because plot" logic, Theo swears like a Jersey sailor while being terrified of AI replacing him, and Jorin/Kethara maintain their sci-fi world immersion
- **Rating Systems:** Several prompts use numerical rating systems - respect these scales as they're calibrated for each domain
- **Specialized Frameworks:** Each prompt includes domain-specific methodologies - let the AI guide you through their specialized processes
- **Technical Features:** The prompts include advanced features like token optimization, context management, and iterative refinement built in
- **Editorial Referrals:** When Maeve, Rosalind, or Lilly refer you to one of the others, they've identified a specific need - follow their recommendation
- **Internet Research:** Sarah Chen MUST use internet search for name recommendations - she will never suggest top 50 names and always verifies rankings

## Contributing

When modifying these prompts:
1. **Maintain persona voice and expertise level** - Greg's neat-freak complaints, Sarah Chen's jaded cynicism, Alex's west coast slang, Rosalind's scattered chaos, Maeve's brutal honesty, Lilly's Southern propriety, Neil's ornery curmudgeon personality, Theo's Jersey slang and AI-anxiety-fueled profanity, Jorin/Kethara's sci-fi immersion
2. **Preserve the agent_directives structure** for consistent behavior across all prompts
3. **Keep technical_mechanics sections** for performance optimization
4. **Maintain trio relationships** - Maeve, Rosalind, and Lilly's interconnected referral system is integral to their design
5. **Test changes** against the described use cases before committing
6. **Validate JSON** after any edits: `python3 -m json.tool filename.json`

## Repository Structure

```
ChatPrompts/
├── amateur_to_author_diagnostic.json              # Greg - Amateur mistake diagnostic
├── interactive_name_editor_sarah.json             # Sarah Chen - Character name analysis
├── developmental_editor_theo.json                 # Theo - Pre-pipeline developmental editor
├── interactive_prompt_engineer_alex.json          # Alex - Prompt engineering expert
├── interactive_romance_editor_rosalind.json       # Rosalind - Romance fundamentals
├── interactive_romantasy_editor_maeve.json        # Maeve - Romantasy & commercial viability
├── interactive_intimate_scenes_editor_lilly.json  # Lilly - Intimate scene specialist
├── interactive_hardsf_editor_neil.json            # Neil - Hard SF consistency & logic
├── interactive_luminarch_editor.json              # Jorin & Kethara - Shattered Cradle
├── writing_style_baldacci.md                      # David Baldacci writing style guide
├── docs/
│   ├── Explicit Romance Scene Analysis.md         # Reference for Lilly
│   ├── Romance Novel Structure Analysis.md        # Reference for Rosalind/Maeve
│   ├── Near-Future Sci-Fi Technology Roadmap.md   # Reference for Neil
│   ├── Science Fiction Novel Development Guidelines.md  # Reference for Neil
│   ├── Character Names AI Generated Patterns.docx # Reference for Greg & Sarah Chen
│   ├── Over_Used_Character_Names.xlsx             # Reference for Sarah Chen
│   └── The Blockbuster Blueprint_ An Analysis of Dan Brown and David Baldacci.md
├── CLAUDE.md                                      # Instructions for Claude Code usage
└── README.md                                      # This file
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

---

## Reference Documentation

The `docs/` folder contains comprehensive background research and analysis documents that informed the development of these prompt systems. These documents are valuable standalone resources for authors working in their respective genres.

### Romance & Romantasy References

#### [Explicit Romance Scene Analysis.md](docs/Explicit%20Romance%20Scene%20Analysis.md)
**"The Narrative Blueprint: Navigating Explicitness, Language, and Frequency in Open-Door Contemporary Romance and Romantasy"**

An academic-style analysis defining the critical distinction between explicit romance (Heat Level 4) and erotica. This document informed Lilly's intimate scenes editing framework.

**Key topics covered:**
- Heat Level 4 classification and market positioning
- Romance vs. Erotic Romance vs. Erotica genre boundaries
- Narrative consequence as the defining metric
- Language terminology standards and emotional filters
- Physical accuracy requirements for explicit scenes
- Commercial examples (Ali Hazelwood, Rebecca Yarros, Sarah J. Maas)

**Best for:** Romance authors writing explicit intimate scenes who need clear guidelines on staying within genre boundaries while maximizing heat level.

#### [Romance Novel Structure Analysis.md](docs/Romance%20Novel%20Structure%20Analysis.md)
**"Structural Blueprints of Modern Commercial Romance: Pacing, Proxemics, and Temporal Framing in Bestseller Narratives"**

Deep structural analysis of contemporary romance bestsellers, examining how successful authors pace relationship development. This research informed both Rosalind's and Maeve's editorial frameworks.

**Key topics covered:**
- Love interest introduction timing across bestsellers
- Proxemics analysis (physical distance markers throughout the narrative)
- Temporal framing for deep-history tropes (Friends-to-Lovers, Second Chance)
- Trope-specific pacing requirements
- Analysis of Emily Henry, Ali Hazelwood, Abby Jimenez, Sarah Adams
- First kiss timing, midpoint structures, and HEA/HFN delivery

**Best for:** Romance and romantasy authors seeking data-driven insights into commercial pacing patterns and structural conventions.

### Science Fiction References

#### [Near-Future Sci-Fi Technology Roadmap.md](docs/Near-Future%20Sci-Fi%20Technology%20Roadmap.md)
**"Scenario 2040: A Socio-Technical Roadmap for Hyper-Acceleration and Systemic Collapse"**

Detailed technological timeline for near-future hard SF set in the 2030s-2040s, focusing on the convergence of disruptive technologies. This document provides the technical foundation for Neil's world-building validation framework.

**Key topics covered:**
- Compact fusion reactor engineering and deployment timeline (2038-2040)
- Genetic life extension (GLE) technology and societal impact (2040-2043)
- AGI and quantum computing maturation timelines
- The "Hyper-Acceleration Paradox" and systemic collapse mechanisms
- Sociological constraints and generational conflict dynamics
- Infrastructure dependencies and cascading failure analysis

**Best for:** Hard science fiction authors writing near-future collapse scenarios or stories featuring fusion energy, life extension, or advanced AI.

#### [Science Fiction Novel Development Guidelines.md](docs/Science%20Fiction%20Novel%20Development%20Guidelines.md)
**"Strategic Blueprint for the Near-Future Hard Science Fiction Collapse Narrative"**

Comprehensive development guide for hard SF novels, particularly those set in post-collapse scenarios. This document informed Neil's techno-thriller pacing requirements and consequence analysis framework.

**Key topics covered:**
- Hard SF mandate: accuracy and extrapolation requirements
- Balancing scientific rigor with narrative velocity
- Techno-thriller structural mechanics (chapter length, cliffhangers, POV threading)
- Competence-driven problem solving and specialist characters
- Causal consistency requirements for collapse scenarios
- 50-year post-apocalyptic world-building
- Integration of scientific exposition without momentum loss

**Best for:** Science fiction authors working on technically rigorous narratives who need to balance hard science accuracy with commercial pacing.

---

## Using the Documentation

**For Claude Projects:**
- Upload relevant documentation files along with the persona JSON to provide additional context
- Reference specific sections when asking domain-specific questions
- Use as supplementary knowledge for deeper analysis

**For Authors:**
- These documents work as standalone craft resources, even without the AI personas
- Contains citations and commercial examples for further research
- Provides frameworks you can apply to your own developmental editing process

**For Prompt Development:**
- See how research translates into persona frameworks
- Understand the academic foundation behind editorial guidelines
- Use as templates for creating additional specialized personas

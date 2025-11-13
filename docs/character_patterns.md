# Character Pattern Integration Analysis

## Review Summary

Three new files have been added containing comprehensive research on AI-detectable patterns in fiction:

### 1. Character Names AI Generated Patterns.docx
- 87 naming patterns across 21 categories
- The "Sarah Chen Complex" - model-specific default characters
- The "Fantasy Troika" - most overused fantasy names (Elara, Lyra, Aria, Kira)
- Phonetic patterns (vowel clustering, consonant patterns)
- Cultural and genetic patterns
- Apostrophe and punctuation abuse
- Gender stereotyping in names
- Historical and literary reference abuse
- Genre-specific patterns
- Cross-model convergence patterns

### 2. Over_Used_Character_Names.xlsx
- **179+ first names** categorized by severity (CRITICAL/HIGH/MEDIUM)
- **70+ last names** with genre-specific overuse
- **55+ problematic name combinations** (alliterative, genre formulas, etc.)
- **150+ trademarked characters** to avoid
- Top offenders:
  - **CRITICAL**: Elara, Lyra, Aria, Kira, Katherine variants, Jack
  - **HIGH**: Marcus, Sarah, Luna, Liam, Ophelia, Orion, Seraphina

### 3. Prohibited_Content_Deep_Dive_Roadmap.xlsx
- 41-category system for AI detection patterns
- Character names ranked as **#1 CRITICAL priority**
- Estimated 3,400-3,800 total prohibited items across all categories
- Priority breakdown:
  - 🔴 CRITICAL Priority: #1-#2 (2 categories)
  - 🟠 HIGH Priority: #3-#12 (10 categories)
  - 🟡 MEDIUM Priority: #13-#29 (17 categories)
  - ⚪ LOW Priority: #30-#41 (12 categories)

---

## Integration Proposal for ClaudeHumanizer

### Option 1: NEW MASTER LIST (Recommended)

Create `master_prohibited_character_patterns.json` as a companion to `master_prohibited_words.json`:

```json
{
  "title": "Master Prohibited Character Patterns List",
  "version": "1.0.0",
  "date": "2025-01-12",
  "description": "Character naming patterns that indicate AI generation",

  "prohibited_first_names": {
    "critical": ["Elara", "Lyra", "Aria", "Kira"],
    "high": ["Elena", "Marcus", "Liam", "Luna"],
    "medium": []
  },

  "prohibited_last_names": {
    "high": ["Chen", "Grey", "Black", "Thorne"],
    "medium": []
  },

  "prohibited_full_names": [
    "Sarah Chen",
    "Marcus Chen",
    "Dr. Chen"
  ],

  "pattern_based_rules": {
    "excessive_vowel_endings": {
      "description": "Female names ending in -a appear 2-3x natural frequency",
      "examples": ["Elara", "Sera", "Kaia", "Thalia"],
      "detection": "Flag if 60%+ of female names end in vowels"
    },

    "el_prefix_overuse": {
      "description": "El- prefix heavily overused in AI fantasy",
      "examples": ["Elara", "Elowen", "Eldoria"],
      "detection": "Flag if 3+ characters start with El-"
    },

    "k_initial_clustering": {
      "description": "Excessive K-initial names in fantasy",
      "examples": ["Kai", "Kael", "Kaelen", "Kira"],
      "detection": "Flag if >15% of names start with K"
    },

    "alliterative_combinations": {
      "description": "Comic book-style alliteration patterns",
      "examples": ["Peter Parker", "Bruce Banner", "Lois Lane"],
      "detection": "Flag if first/last names share initial letter"
    },

    "phonetic_rhyming": {
      "description": "Multiple characters with rhyming endings",
      "examples": ["Elara/Lyra/Kira", "Thorne/Corne/Sorne"],
      "detection": "Flag if 2+ names share -ra/-la/-or endings"
    }
  },

  "cultural_pattern_warnings": [
    {
      "pattern": "Chen + non-Asian context",
      "severity": "CRITICAL",
      "example": "Marcus Chen as white supremacist leader"
    },
    {
      "pattern": "Rodriguez overuse",
      "severity": "MEDIUM",
      "note": "Default Hispanic surname - use diverse alternatives"
    }
  ],

  "phonetic_analysis_rules": {
    "vowel_percentage_female": {
      "natural_range": "35-45%",
      "ai_typical": "50%+",
      "action": "Flag names with 50%+ vowel content"
    },

    "high_front_vowels": {
      "description": "Overuse of /i/ and /e/ sounds",
      "ai_examples": ["Elara", "Elise", "Elaine", "Iris", "Erin"],
      "action": "Flag if 60%+ of names contain i/e vowels"
    }
  }
}
```

**Integration points:**
- **Phase 2 (AI Word Cleaning)**: Add character name detection as new subsection
- **Phase 6 (Dialogue Enhancement)**: Check speaker attribution names
- **Phase 9 (Final Verification)**: Add character name pattern analysis
- **Phase 10 (Final AI Word Sweep)**: Catch any reintroduced problematic names

---

### Option 2: NEW PHASE 6.2 - Character Name Audit

Insert after Phase 6.1 (Character Dialogue Pass) as optional phase:

**`6.2_character_name_audit.json`**
- Scans all character names in manuscript
- Checks against prohibited name lists
- Flags phonetic patterns (El- prefix, -a endings, K-clustering)
- Analyzes cultural consistency
- Provides replacement suggestions
- **Domain**: Character names ONLY (respects domain isolation)

---

### Option 3: PHASE 9 ENHANCEMENT

Add character name analysis to existing Phase 9 (Final Verification):

Current Phase 9 checks:
- N-grams
- Perplexity phrases
- AI pattern detection

**Add new subsection:**
```json
"character_name_analysis": {
  "instructions": [
    "Scan all character names in the text",
    "Flag names from prohibited_character_patterns.json",
    "Check for phonetic clustering (El-, K-, -a endings)",
    "Verify cultural consistency of name combinations",
    "Report findings WITHOUT modifying text"
  ]
}
```

---

### Option 4: REFERENCE DOCUMENTATION

Convert to markdown reference documents (no automated checking):

- `docs/CHARACTER_NAMING_GUIDE.md` - Writer education
- `docs/AI_PATTERN_DETECTION_REFERENCE.md` - Full 41-category roadmap
- Keep as manual checklist for writers to self-audit

---

## Recommended Implementation Strategy

### Phase 1: Immediate (Character Names)

1. **Create `master_prohibited_character_patterns.json`** from Excel data
2. **Update Phase 2** to include character name checking:
   ```json
   "character_name_detection": {
     "check_against": "master_prohibited_character_patterns.json",
     "action": "Replace prohibited names with alternatives"
   }
   ```
3. **Update Phase 9** to report (not fix) any remaining problematic names
4. **Create documentation**: `docs/CHARACTER_NAMING_PATTERNS.md`

### Phase 2: Future (Broader Patterns)

1. **Expand roadmap categories #2-#12** (HIGH priority) into master list
2. **Add pattern detection** to relevant phases:
   - **Phase 3**: Purple prose (already covers "delve, tapestry, realm")
   - **Phase 7**: Weak language/transitions (add "furthermore, moreover")
   - **Phase 9**: Structural patterns ("It's not X, it's Y" constructions)

3. **Create optional Phase 9.6**: "Content Pattern Analysis"
   - Checks for plot tropes, clichés, structural tells
   - Reports findings for manual review
   - Does NOT modify text (analysis only)

### Phase 3: Long-term (Full System)

Build out all 41 categories from roadmap as reference material and optional detection modules.

---

## Why Character Names Should Be Priority #1

The roadmap correctly identifies character names as CRITICAL:

✅ **Most visible AI marker** - readers notice immediately
✅ **Easiest to fix** - simple find/replace operation
✅ **Statistical evidence** - documented patterns (Elara appears 15+ times, Sarah Chen 90%+ frequency)
✅ **Instant detection** - "Elara" immediately flags AI-generated content
✅ **Domain-compatible** - fits ClaudeHumanizer's assembly line architecture

---

## Key Research Findings

### The "Sarah Chen" Phenomenon

The most notorious example of AI naming predictability:
- Appears across ChatGPT, Claude, Gemini, DeepSeek with 90%+ frequency
- Used in wildly different contexts (researcher, developer, analyst, educator)
- Reveals model's inability to generate authentic diversity

**Why this happens:**
- Sarah = 2nd most frequent female character name in films
- Chen = one of most common surnames globally
- Combination creates statistically powerful "default expert" archetype
- Common names require fewer tokens (computationally "cheaper")

### Vowel-Heavy Feminine Name Pattern

AI systems disproportionately generate female names ending in vowels:
- Natural frequency in English: 37%
- AI-generated frequency: 60-90%
- Names like Elara, Aria, Lyra, Kira appear in 80-90% of AI fantasy stories

### Phonetic Patterns

**El- Prefix Overuse:**
- Elara, Elena, Elowen, Eldoria
- Treated as "quasi-fantasy" marker by AI

**K-Initial Clustering:**
- Kai, Kael, Kaelen, Kira
- AI generates excessive K-names for fantasy

**Hard vs. Soft Consonants:**
- Male names: Marcus, Kai, Kale, Thorne, Aldric (harsh consonants)
- Female names: Aria, Elara, Sera (soft sounds)
- Reflects training data gender stereotyping

---

## Critical Names to Avoid

### CRITICAL Severity (Instant AI Flags)

**First Names:**
- Elara, Lyra, Aria, Kira (Fantasy Troika + Kira)
- Katherine/Kate/Katie/Caitlin/Katniss (all variants)
- Jack (most popular male name in all literature)

**Full Names:**
- Sarah Chen
- Marcus Chen
- Dr. Chen
- Elena (any context)

### HIGH Severity (Very Common AI Patterns)

**First Names:**
- Marcus, Elias, Orion, Adrian (male)
- Luna, Ophelia, Seraphina, Freya (female)
- Emma, Olivia, Ava, Grace (contemporary)
- Liam, Noah, Ethan, Gabriel (romance)

**Last Names:**
- Chen (any combination)
- Grey, Black, Thorne
- Smith, Jones (generic defaults)

**Genre-Specific:**
- Dante, Dominic (Mafia/Dark Romance)
- Ivan, Mikhail (Bratva Romance)
- Hudson, Landon (YA/Paranormal)

---

## Pattern-Based Detection Rules

### 1. Excessive -a Endings (Female Names)
- **Flag if**: 60%+ of female characters have names ending in -a
- **Examples**: Elara, Lyra, Aria, Kaida, Sera, Lena, Elena, Sienna, Kira, Raya

### 2. El- Prefix Clustering
- **Flag if**: 3+ characters start with "El-"
- **Examples**: Elara, Elena, Elise, Elaine, Elowen, Eldoria

### 3. K-Initial Overuse
- **Flag if**: >15% of names start with K
- **Examples**: Kai, Kael, Kaelen, Kira, Kale

### 4. Rhyming Cascade
- **Flag if**: 2+ names share rhyming endings
- **Examples**: Elara/Lyra/Kira/Sera, Thorne/Corne/Sorne

### 5. Alliterative Combinations
- **Flag**: First and last names sharing initial letter
- **Examples**: Peter Parker, Bruce Banner, Lois Lane

### 6. Cultural Inconsistency
- **Flag**: Chen paired with non-Asian context
- **Flag**: Generic "Fantasy Elf" names used for all species

### 7. Vowel Percentage Anomalies
- **Natural range**: 35-45% vowel content
- **AI typical**: 50%+ vowel content
- **Flag**: Names with 50%+ vowels (hyper-feminine sound)

### 8. High Front Vowel Overuse
- **Flag if**: 60%+ of names contain /i/ or /e/ sounds
- **Examples**: Elara, Elise, Elaine, Iris, Erin

---

## Integration Decision Points

**Choose one approach:**

1. **Create `master_prohibited_character_patterns.json`** + enhance existing phases ← RECOMMENDED
2. **Create new Phase 6.2** (Character Name Audit)
3. **Add to Phase 9 only** (reporting, not fixing)
4. **Documentation/reference only** (no automation)

**Next steps available:**
- Convert Excel → JSON
- Write new phase prompts
- Update existing phase prompts
- Create documentation
- Validate against `PROMPT_TEMPLATE.json`

---

## 41-Category Roadmap Overview

### 🔴 CRITICAL Priority (#1-#2)
1. **Character Names** - AI-Generated Patterns (175-200 names)
2. **Overused Descriptive Words & Purple Prose** (150-200 words)

### 🟠 HIGH Priority (#3-#12)
3. Cliché Phrases & Transitions (100-150 phrases)
4. AI Writing Structures & Patterns (50-75 patterns)
5. Plot Tropes & Story Clichés (80-120 tropes)
6. Academic/Formal Writing Markers (120-180 phrases)
7. Linguistic & Statistical Patterns (30-50 patterns)
8. Hedging & Neutral Language (40-60 phrases)
9. Structural & Formatting Tells (30-45 tells)
10. Parallelism & Repetitive Constructions (30-50 structures)
11. Content Depth Issues (40-60 issues)
12. Missing Natural Elements (40-60 elements)

### 🟡 MEDIUM Priority (#13-#29)
13. Character Archetypes & Stereotypes (60-90 archetypes)
14. Romance/Relationship Tropes (70-100 tropes)
15. Conflict & Stakes Patterns (40-60 types)
16. Emotional Description Patterns (80-120 descriptors)
17. Opening Lines & Hooks (40-60 formulas)
18. Closing Phrases & Conclusions (30-50 patterns)
19. World-Building Terms (100-150 terms)
20. Action Scene Clichés (60-90 clichés)
21. Voice & Consistency Issues (25-40 issues)
22. Citation & Reference Patterns (20-35 patterns)
23. Too Much Perfection (20-30 indicators)
24. Quick Response & Placeholder Text (20-30 tells)
25. Jargon & Vocabulary Misuse (50-75 examples)
26. Question & Answer Formatting (20-30 patterns)
27. Chapter Ending Patterns (40-60 patterns)
28. Metaphor & Simile Overuse (100-150 comparisons)
29. Timestamp & Context Mismatches (30-50 mismatches)

### ⚪ LOW Priority (#30-#41)
30. Power System Clichés (50-75 clichés)
31. Dialogue Tags & Attribution (50-80 tags)
32. Scene Transition Phrases (40-60 phrases)
33. Time/Setting Descriptions (50-80 descriptors)
34. Multiple Reasons/Evidence Overload (25-40 patterns)
35. Grammar & Punctuation Quirks (30-50 quirks)
36. Emoji & Symbol Patterns (15-25 patterns)
37. Marketing/Business Buzzwords (200-300 terms)
38. Visual Content Detection Patterns (50-75 tells)
39. Audio/Speech Patterns (30-40 tells)
40. False Attribution Patterns (20-35 errors)
41. Social Media Specific Tells (20-30 patterns)

**Grand Total**: ~3,400-3,800 prohibited items across all categories

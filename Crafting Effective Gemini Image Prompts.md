# **The Semantics of Vision: A Comprehensive Methodology for High-Fidelity Image Generation with Gemini 3 Pro ("Nano Banana Pro")**

## **Executive Summary**

The advent of Gemini 3 Pro Image—internally and colloquially recognized within the developer community as "Nano Banana Pro"—marks a definitive schism in the trajectory of generative Artificial Intelligence. While preceding generations of image synthesis models, such as latent diffusion architectures, relied primarily on stochastic token association to approximate visual outputs, Gemini 3 Pro introduces a "reasoning engine" into the generation pipeline.1 This shift moves the discipline of prompt engineering from a practice of "keyword curation" to one of "semantic orchestration."

This report provides an exhaustive analysis of the methodologies required to master this specific architecture. It is designed to bridge the gap between the user’s established prompting framework—comprising **Background, Subject, Composition, Action, Location, and Style**—and the advanced capabilities of the Gemini 3 Pro reasoning engine. Through a synthesis of technical documentation, developer logs, and expert user case studies, this document establishes a rigorous protocol for "Semantic Blueprinting."

The analysis reveals that while the user’s current six-section structure is directionally correct, it requires significant deepening to leverage the model’s unique ability to "think" before it renders. We explore the critical debate between Natural Language and Structured Data (JSON) prompting, ultimately proposing a hybrid workflow that utilizes autonomous "Creative Director" agents to draft rigorous JSON schemas. This report aims to serve as the definitive operational manual for creating production-grade, logically sound, and aesthetically superior visual assets using Google’s most advanced multimodal system.

## ---

**1\. The Paradigm Shift: From Stochastic Diffusion to Multimodal Reasoning**

To develop a robust method for prompting Gemini 3 Pro, it is essential to first deconstruct the architectural evolution that distinguishes it from its predecessors. This understanding allows the prompt engineer to align their instructions with the model's internal processing logic, thereby minimizing hallucinations and maximizing fidelity.

### **1.1 The Architecture of "Nano Banana Pro"**

Gemini 3 Pro Image (Nano Banana Pro) is not merely a larger diffusion model; it is a natively multimodal system underpinned by a reasoning backbone. Traditional text-to-image models operate by encoding text into vector embeddings (using encoders like CLIP) and then guiding a denoising process to match those vectors. This often results in a "bag-of-words" interpretation where the model understands "astronaut" and "horse" but struggles with "astronaut riding a horse," often producing a horse riding an astronaut due to a lack of syntactic comprehension.

In contrast, Gemini 3 Pro utilizes a "Thinking Process".3 When a prompt is received, the model engages in an internal chain-of-thought sequence—a latent phase where it plans the composition, resolves logical conflicts, and verifies physical constraints before a single pixel is rendered.4 This "Thinking" capability allows the model to interpret intent beyond mere keyword matching. For example, if a user requests an image of a "melting chess set made of ice on a lava board," the reasoning engine calculates the thermodynamic interactions—steam generation, water pooling, and light refraction—rather than simply pasting "ice" and "fire" textures adjacent to one another.4

### **1.2 The "Thinking" Mechanism and Prompt Adherence**

The "Thinking" mode, accessible via the API and advanced interfaces, represents a fundamental change in how prompts should be constructed. In legacy models, brevity was often preferred to prevent "confusing" the model. With Gemini 3 Pro, the "Thinking" mechanism thrives on context and complexity.5

The implications for the user’s methodology are profound. The model does not just "see" the prompt; it "reads" it. It analyzes the causal relationships between the *Subject*, *Action*, and *Environment*. Therefore, the prompt must function less like a list of tags (e.g., "4k, realistic, dog") and more like a creative brief or a screenplay.6 The reasoning engine uses this brief to generate intermediate "thought signatures"—encrypted representations of the planned image structure—which guide the final generation.7 This allows for "one-shot" success on complex logic puzzles, such as ensuring a reflection in a mirror matches the subject's expression, or that text within the image is spelled correctly.1

### **1.3 World Knowledge and Grounding**

A unique differentiator of the Gemini ecosystem is its integration with Google Search for "Grounding".2 Unlike closed-system models that rely solely on training data (which has a knowledge cutoff), Gemini 3 Pro can verify facts in real-time. If a prompt requests a "scientifically accurate cross-section of a V8 engine" or a "historical depiction of a Victorian watchmaker's shop," the model can reference external data to ensure the arrangement of pistons or the style of the lathe is accurate.2 This necessitates a "Location" section in the prompt that is not just aesthetic but *factual*, explicitly invoking the model's world knowledge capabilities.

## ---

**2\. Theoretical Framework: The Psychology of the Prompt**

Before upgrading the user's specific sections, we must address the theoretical underpinnings of why certain prompts fail and others succeed. This centers on the concepts of "Concept Bleeding" and "Token Attention," which are the primary adversaries of clean image generation.

### **2.1 The Phenomenon of Concept Bleeding**

"Concept Bleeding" occurs when the attributes of one object in a prompt leak into adjacent objects.9 For instance, a prompt describing "a woman in a red dress holding a blue umbrella" might result in a purple dress or a red umbrella. This happens because standard attention mechanisms in diffusion models struggle to strictly bind adjectives (red, blue) to their respective nouns (dress, umbrella) when the semantic distance is short.

In the user’s current workflow, simply listing "Background: Red Wall" and "Subject: Blue Suit" in a continuous block of text risks this bleeding. The reasoning engine of Gemini 3 Pro is more robust against this, but it is not immune. To fully mitigate this, we must employ "Variable Isolation"—a technique that separates distinct elements into discrete data chunks.11

### **2.2 Variable Isolation: Natural Language vs. JSON**

There is a significant divergence in expert opinion regarding the best method to enforce variable isolation.

* **The Natural Language School:** Advocates argue that because Gemini is an LLM, it understands nuance. They suggest using full sentences and grammatical structures to separate concepts (e.g., "The woman is wearing a blue suit. In contrast, the wall behind her is red.").6 This approach relies on the "Creative Director" persona, where the user speaks to the model as a colleague.13  
* **The Structured Data (JSON) School:** Proponents argue that "token confusion" is best solved by forcing the model to parse the prompt as a structured dataset.11 By using JSON (JavaScript Object Notation), users can encapsulate "Subject" and "Background" in separate brackets { }, physically and syntactically isolating the tokens. Research indicates this method is superior for "production-grade" assets where consistency is paramount.11

Synthesis for the User:  
To satisfy the user's request for a "good method," we must not choose one over the other but integrate them. We propose a Hybrid Methodology: utilizing Natural Language for the creative ideation phase (the "Action" and "Style") and Structured JSON for the technical execution phase (the "Composition" and "Subject"). This ensures the "soul" of the image is captured by the LLM while the "physics" are constrained by the data structure.

## ---

**3\. The "Semantic Blueprint": Upgrading the User's Six Sections**

The user currently utilizes six sections: **Background, Subject, Composition, Action, Location, Style**. This section of the report deconstructs each of these components, identifies their limitations in their current form, and upgrades them into a "Semantic Blueprint" optimized for Gemini 3 Pro.

### **3.1 Subject: From "Who" to "Identity & Materiality"**

Current Limitation: A simple "Subject" description (e.g., "a robot") leaves too much to interpretation, often resulting in generic "plastic" textures or inconsistent character designs.  
The Upgrade: The "Subject" section must define Materiality ("MadeOutOf") and Identity Locking.

* **Material Physics ("MadeOutOf"):** Gemini 3 Pro’s rendering engine simulates light interaction. To avoid the "AI sheen," the prompt must define the microscopic surface properties. Instead of "a robot," the prompt should specify: *"Subject made of brushed aluminum with micro-scratches and oxidized copper joints. Surface finish is matte, absorbing light rather than reflecting it."*.11  
* **Identity Consistency:** The model supports up to **14 reference images**.2 For consistent characters, the "Subject" section should not just describe the person but reference an uploaded asset. *"Use Reference Image A for facial structure and Reference Image B for clothing style."* This "Few-Shot Prompting" capability ensures the same character can be generated across multiple scenes.2

**Operational Prompt (Subject):**

Subject: A stoic elderly mechanic.  
Materiality: Skin texture is weathered, with visible pores and grease stains. Clothing is heavy denim canvas, frayed at the seams.  
Reference: Use \`\` for facial topology.

### **3.2 Action: From "Verb" to "Kinematics & Causality"**

Current Limitation: Simple verbs (e.g., "running") often result in static figures that look like they are posing.  
The Upgrade: The "Action" section must focus on Kinematics (the study of motion) and Causality (cause and effect).

* **Cinematic Verbs:** The model responds to "high-energy" verbs that imply vectors. Instead of "running," use *"sprinting," "lunging,"* or *"careening."*.17  
* **Causality:** Describe the *effect* of the action on the environment to ground the subject. *"Mid-stride, kicking up a spray of water from the puddle. The coat tails are whipping violently behind due to wind resistance."* This forces the reasoning engine to calculate fluid dynamics and wind physics.15

**Operational Prompt (Action):**

Action: Vaulting over a concrete barrier.  
Kinematics: Body is fully extended, muscles tensed.  
Causality: Debris is displaced by the impact of the trailing foot; dust hangs in the air along the trajectory.

### **3.3 Composition: From "Framing" to "Virtual Cinematography"**

Current Limitation: Terms like "close-up" are subjective.  
The Upgrade: The "Composition" section must simulate a Virtual Camera, defining lens focal length, aperture, and sensor type.

* **Lens Selection:** The model understands optical physics.  
  * *35mm / 24mm:* Use for environmental storytelling; widens the field of view.18  
  * *85mm / 100mm:* Use for portraits; compresses features and flatters the subject.18  
  * *Macro:* Use for texture details; enforces extreme close-focus.4  
* **Aperture (Depth of Field):** Defining the f-stop controls the bokeh. *"f/1.8"* creates a shallow depth of field (blurry background), separating the subject. *"f/16"* ensures deep focus where everything is sharp.11  
* **Aspect Ratio:** Explicitly state the canvas dimensions (e.g., *16:9, 21:9*) to ensure the composition is framed correctly from the start.1

**Operational Prompt (Composition):**

Camera: Virtual Arri Alexa.  
Lens: 50mm Prime.  
Aperture: f/2.8.  
Framing: Dutch angle, rule of thirds, subject in right quadrant.  
Aspect Ratio: 2.39:1 (Cinematic Anamorphic).

### **3.4 Location: From "Place" to "Grounding & World Knowledge"**

Current Limitation: Generic locations (e.g., "a coffee shop") yield generic, hallucinated details.  
The Upgrade: The "Location" section should leverage Grounding to pull specific, factual details from the model's knowledge base.

* **Factual Anchoring:** Use specific names. *"A coffee shop in Shibuya, Tokyo."* The model will generate accurate signage, outlet types, and architectural nuances specific to that region.4  
* **Historical Accuracy:** *"A 1920s Speakeasy."* The model effectively ignores modern elements (LEDs, plastic) and populates the scene with period-correct glassware and Art Deco patterns.2  
* **Atmosphere:** Define the "air" of the location. *"Filled with volumetric fog and cigarette smoke,"* or *"Sterile, vacuum-sealed environment."*

**Operational Prompt (Location):**

Location: A subway station in 1980s New York City.  
Grounding: Accurately reflect the graffiti style and subway car design of the era.  
Atmosphere: Gritty, humid, subterranean haze.

### **3.5 Background: From "Setting" to "Global Illumination"**

Current Limitation: "Background" often overlaps with "Location."  
The Upgrade: Redefine "Background" to focus on Global Illumination (Lighting) and Context.

* **Lighting Physics:** Light dictates the mood.  
  * *Hard Light:* "Direct flash," "Noon sun." Creates sharp, high-contrast shadows.19  
  * *Soft Light:* "Window light," "Overcast," "Softbox." Wraps around the subject.11  
  * *Color Temperature:* "Warm tungsten" (orange/cozy) vs. "Cool fluorescent" (blue/sterile).19  
* **Separation:** Explicitly instruct the background to be visually distinct from the subject to prevent blending. *"Background is out of focus and darker than the subject."*

**Operational Prompt (Background/Lighting):**

Lighting: Golden hour backlighting.  
Source: Low sun angle creates long shadows.  
Tone: Warm, amber hues interacting with cool ambient skylight.

### **3.6 Style: From "Vibe" to "Aesthetic Anchor"**

Current Limitation: Vague terms like "cool" or "pretty" are non-functional.  
The Upgrade: The "Style" section must act as an Aesthetic Anchor, referencing specific media, artists, or rendering engines.

* **Medium Simulation:** *"Shot on Kodak Portra 400"* (adds film grain and specific color science).18 *"Oil painting with heavy impasto"* (adds texture). *"Unreal Engine 5 Render"* (adds digital sharpness and ray-tracing).  
* **Negative Constraints:** Use the "Style" section to define what the image is *not*. *"No 3D render, no cartoon, no illustration."*.16

**Operational Prompt (Style):**

Style: Neo-Noir Cyberpunk.  
Reference: Blade Runner aesthetics.  
Medium: Digital Photography, high ISO grain.

## ---

**4\. Advanced Methodology: The JSON Protocol**

While the natural language approach is intuitive, the research strongly suggests that **JSON Prompting** is the optimal method for leveraging Gemini 3 Pro’s reasoning capabilities, particularly for preventing concept bleeding.11 This section translates the user's upgraded six sections into a rigorous JSON schema.

### **4.1 The Case for Structured Data**

The argument that JSON adds "noise" 12 is predicated on older models that processed text line-by-line. Gemini 3 Pro, however, is trained on vast repositories of code and structured data. It "thinks" in logic. By using JSON, the user provides a "form" rather than a "story," which forces the model to categorize tokens strictly.

* **Benefit 1:** *Isolation.* "Subject" attributes cannot bleed into "Background" attributes because they are enclosed in separate braces {}.  
* **Benefit 2:** *Editability.* Changing the time\_of\_day key from "day" to "night" updates the entire lighting model without requiring a rewrite of the subject description.14

### **4.2 The "Nano Banana Pro" Master Schema**

The following JSON structure integrates the user's six sections (mapped to technical keys) into a format optimized for the Gemini API and advanced interface.

JSON

{  
  "meta\_data": {  
    "project\_label": "Campaign\_X\_Hero\_Image",  
    "aspect\_ratio": "16:9",  
    "quality\_preset": "Ultra-High Fidelity"  
  },  
  "semantic\_blueprint": {  
    "subject\_block": {  
      "identity": "A sophisticated elderly mechanic",  
      "materiality\_physics":,  
      "pose\_kinematics": "Leaning forward, inspecting a gear, muscles tense",  
      "reference\_id": "image\_upload\_01"  
    },  
    "environment\_block": {  
      "location\_grounding": "Victorian Watchmaker Shop (1890s historical accuracy)",  
      "background\_elements":,  
      "atmosphere": "Claustrophobic but cozy, filled with ticking sounds (visualized as motion blur)"  
    },  
    "virtual\_camera": {  
      "lens\_focal\_length": "85mm (Portrait)",  
      "aperture": "f/1.8 (Shallow Depth of Field)",  
      "angle": "Eye-level",  
      "focus\_point": "Subject's eyes"  
    },  
    "lighting\_simulation": {  
      "type": "Rembrandt Lighting",  
      "sources":,  
      "shadows": "Deep, soft-edged"  
    },  
    "style\_anchor": {  
      "aesthetic": "Steampunk Realism",  
      "medium": "Digital Photography",  
      "film\_stock": "Kodak Portra 400 (simulated grain)"  
    },  
    "negative\_constraints": \[  
      "No plastic textures",  
      "No distorted hands",  
      "No text overlays",  
      "No modern technology"  
    \]  
  }  
}

### **4.3 Implementing the JSON Workflow**

1. **Drafting:** The user does not need to write this manually. They can use a "Creative Director" Agent (see Section 6\) to generate this JSON based on a simple idea.  
2. **Execution:** Paste this block directly into the Gemini "Thinking" model prompt box.  
3. **Iteration:** To change the scene, simply modify the environment\_block values while keeping subject\_block identical. This ensures perfect character consistency across different locations.19

## ---

**5\. Specialized Capabilities: Text, Infographics, and Reference Fusion**

Gemini 3 Pro offers capabilities that go beyond standard "image generation." These features require specific prompting techniques to unlock.

### **5.1 Text Rendering and Typography**

Unlike previous models that produced gibberish, Gemini 3 Pro uses an enhanced text encoder to render legible text.1

* **Technique:** Use explicit quoting and location commands.  
* **Prompt:** *"Generate a neon sign that says **'OPEN 24 HOURS'**. The text must be strictly legible, spelled correctly, and centered. Font style: Sans-serif bold."*.4  
* **Localization:** The model can translate text within the image. *"Translate the sign to Japanese Kanji."*.4

### **5.2 Infographics and Data Visualization**

The reasoning engine allows for the logical arrangement of information.15

* **Technique:** Define "Logical Layout Anchors."  
* **Prompt:** *"Create a vertical infographic about the Water Cycle. Top Section: 'Evaporation' with cloud icons. Middle Section: 'Condensation'. Bottom Section: 'Precipitation'. Ensure arrows connect the sections logically."*  
* **Insight:** The model "plans" the space to prevent text overlap, a capability unique to its "Thinking" mode.20

### **5.3 Reference Image Fusion (The 14-Image Input)**

The ability to ingest up to 14 reference images is a game-changer for branding.2

* **Technique:** Role assignment.  
* **Prompt:** *"Use Image 1 and 2 for the Subject's face. Use Image 3 for the lighting style. Use Image 4 for the color palette. Blend these inputs to create a cohesive new image."*  
* **Application:** This allows for "Virtual Try-On" (putting a specific shirt on a specific model) or "Style Transfer" (applying a Van Gogh style to a photograph) with high precision.8

## ---

**6\. The Agentic Future: "Creative Director" Workflows**

To maximize efficiency, the user should move from manual prompting to **Agentic Orchestration**. This involves using a text-based AI (like Gemini 1.5 Pro or GPT-4) to act as a "middleman" that writes the complex prompts for the image model.

### **6.1 The "Creative Director" Persona**

The user should set up a saved prompt or "Gem" in their text AI with the following System Instruction:

**System Prompt:** "You are an expert AI Creative Director. Your goal is to translate simple user concepts into high-fidelity JSON prompts for the Gemini 3 Pro Image model. You must use the 'Semantic Blueprint' structure, ensuring detailed descriptions for Materiality, Kinematics, Virtual Camera, and Global Illumination. Always output the result in the defined JSON schema.".13

### **6.2 Antigravity and Coding Agents**

For advanced users, Google's **Antigravity** IDE allows for "Agent-First" development.21 Users can build workflows where a coding agent automatically generates UI mockups using Gemini 3 Pro.

* **Workflow:** The user types "Design a login screen for a fitness app." The Antigravity agent uses Gemini 3 Pro to generate the image, then writes the React code to match the image.22 This represents the convergence of design and development, facilitated by the "Thinking" model's ability to understand UI logic.

## ---

**7\. Sector-Specific Application Scenarios**

To demonstrate the versatility of this method, we apply the "Semantic Blueprint" to three distinct professional domains.

| Sector | Scenario | Key Prompting Strategy |
| :---- | :---- | :---- |
| **E-Commerce** | **Product Photography** | **Reference Locking \+ Lighting Physics.** Use reference\_id to ensure the product is exact. Use lighting\_simulation to create "studio softbox" effects that highlight textures (e.g., leather grain). |
| **Architecture** | **Interior Visualization** | **Grounding \+ Virtual Camera.** Use location\_grounding to ensure furniture is scale-accurate. Use lens\_focal\_length: 24mm to capture the room width without distortion. |
| **Marketing** | **Global Campaign** | **Text Rendering \+ Localization.** Generate a base ad with the text "SALE" in English. Use the edit function to generate variants where the text is "VENTE" (French) or "VENTA" (Spanish) while keeping the background identical.2 |

## ---

**8\. Operational Best Practices: The "Pro" Protocol**

To conclude, we distill the research into a set of operational rules for the user to follow.

1. **Always Enable "Thinking":** If the interface allows, ensure the model is in "Thinking" or "Reasoning" mode. This adds latency but significantly improves adherence to complex logic.3  
2. **Edit, Don't Re-roll:** When an image is close, do not generate a new one. Use the conversational interface to refine it. *"Make the light warmer"* is cheaper and more effective than re-running the full prompt.5  
3. **Negative Constraints are Mandatory:** Always include a negative\_constraints block to filter out common AI artifacts (e.g., "extra fingers," "blurry text," "floating objects").  
4. **Audit the "Thought Signatures":** In API usage, capture the "thought\_signature" returned by the model. Passing this signature back in subsequent turns helps the model "remember" its reasoning, ensuring consistency in multi-turn edits.7

By adopting this **Semantic Blueprint**—which upgrades the user's six sections into a sophisticated, data-driven framework—and leveraging the hybrid power of Natural Language creativity and JSON structural integrity, the user can unlock the full potential of Gemini 3 Pro. This is not just about making "good" images; it is about establishing a predictable, professional, and scalable visual production pipeline.

## ---

**9\. Appendix: Detailed Implementation Guide for the Six Sections**

This section provides a granular, step-by-step expansion of the user's six original sections, populated with data table references and specific parameter values derived from the research.

### **9.1 Table of Recommended "Virtual Camera" Settings**

| Lens Type | Focal Length | Use Case | Prompt Keyword |
| :---- | :---- | :---- | :---- |
| **Ultra-Wide** | 14mm \- 24mm | Architecture, Landscapes | "Expansive," "Distorted edges" |
| **Wide** | 35mm | Street Photography, Environmental Portraits | "Contextual," "Storytelling" |
| **Standard** | 50mm | Natural Vision, Product Shots | "Human eye view," "Natural" |
| **Portrait** | 85mm | Headshots, Character Focus | "Flattering," "Compressed" |
| **Telephoto** | 200mm+ | Sports, Wildlife, Compression | "Background compression," "Flat" |
| **Macro** | 100mm Macro | Textures, Insects, Jewelry | "Micro-details," "1:1 magnification" |

### **9.2 Table of Lighting Physics**

| Lighting Style | Visual Effect | Emotional Tone |
| :---- | :---- | :---- |
| **Golden Hour** | Long shadows, warm orange hue | Nostalgic, romantic, peaceful |
| **Blue Hour** | Low contrast, deep blue hue | Melancholic, serene, cinematic |
| **Hard Flash** | Sharp shadows, high contrast, bleached skin | Gritty, paparazzi, raw, energetic |
| **Rembrandt** | Triangular highlight on cheek, dark shadows | Dramatic, classic, moody |
| **Diffused/Softbox** | No hard shadows, even illumination | Professional, commercial, clean |

These tables should be used as "lookup charts" when populating the virtual\_camera and lighting\_simulation blocks of the JSON prompt.

---

Note: This report synthesizes information from the provided research snippets, specifically.1

#### **Works cited**

1. Nano Banana Pro: Google's New Dominant Image Generation Model \- DataCamp, accessed December 18, 2025, [https://www.datacamp.com/tutorial/nano-banana-pro](https://www.datacamp.com/tutorial/nano-banana-pro)  
2. Nano Banana Pro available for enterprise | Google Cloud Blog, accessed December 18, 2025, [https://cloud.google.com/blog/products/ai-machine-learning/nano-banana-pro-available-for-enterprise](https://cloud.google.com/blog/products/ai-machine-learning/nano-banana-pro-available-for-enterprise)  
3. Nano Banana Pro \- Gemini AI image generator & photo editor, accessed December 18, 2025, [https://gemini.google/overview/image-generation/](https://gemini.google/overview/image-generation/)  
4. The Ultimate Nano Banana Pro Prompting Guide: Mastering Gemini 3 Pro Image \- Atlabs AI, accessed December 18, 2025, [https://www.atlabs.ai/blog/the-ultimate-nano-banana-pro-prompting-guide-mastering-gemini-3-pro-image](https://www.atlabs.ai/blog/the-ultimate-nano-banana-pro-prompting-guide-mastering-gemini-3-pro-image)  
5. The Complete Guide to Nano Banana Pro: 10 Tips for Professional ..., accessed December 18, 2025, [https://antigravityide.org/blog/the-complete-guide-to-nano-banana-pro-10-tips-for-professional-asset-production/](https://antigravityide.org/blog/the-complete-guide-to-nano-banana-pro-10-tips-for-professional-asset-production/)  
6. The Complete Guide to Nano Banana Pro\_ 10 Tips for Professional Asset Production \- Google Antigravity IDE \- Scribd, accessed December 18, 2025, [https://www.scribd.com/document/963481350/The-Complete-Guide-to-Nano-Banana-Pro-10-Tips-for-Professional-Asset-Production-Google-Antigravity-IDE](https://www.scribd.com/document/963481350/The-Complete-Guide-to-Nano-Banana-Pro-10-Tips-for-Professional-Asset-Production-Google-Antigravity-IDE)  
7. Gemini 3 Developer Guide | Gemini API \- Google AI for Developers, accessed December 18, 2025, [https://ai.google.dev/gemini-api/docs/gemini-3](https://ai.google.dev/gemini-api/docs/gemini-3)  
8. Nano Banana Pro: Next-Gen AI in Adobe Firefly, accessed December 18, 2025, [https://www.adobe.com/products/firefly/partner-models/google-gemini-nano-banana.html](https://www.adobe.com/products/firefly/partner-models/google-gemini-nano-banana.html)  
9. Optimizing Multi-Concept Text-to-Image Generation Training-Freely with Isolated Diffusion Guidance \- arXiv, accessed December 18, 2025, [https://arxiv.org/abs/2403.16954](https://arxiv.org/abs/2403.16954)  
10. Prompting HACKS no-one talks about \- sdxlturbo.ai, accessed December 18, 2025, [https://sdxlturbo.ai/blog-Prompting-HACKS-noone-talks-about-29396](https://sdxlturbo.ai/blog-Prompting-HACKS-noone-talks-about-29396)  
11. Nano Banana Pro JSON Prompting Guide: Master Structured AI Image Generation, accessed December 18, 2025, [https://www.atlabs.ai/blog/nano-banana-pro-json-prompting-guide-master-structured-ai-image-generation](https://www.atlabs.ai/blog/nano-banana-pro-json-prompting-guide-master-structured-ai-image-generation)  
12. Does JSON Prompting Actually Work? Tested with Nano Banana | Chase Jarvis, accessed December 18, 2025, [https://chasejarvis.com/blog/does-json-prompting-actually-work-tested-with-nano-banana/](https://chasejarvis.com/blog/does-json-prompting-actually-work-tested-with-nano-banana/)  
13. AI Creative Director \- AI Prompt \- DocsBot AI, accessed December 18, 2025, [https://docsbot.ai/prompts/creative/ai-creative-director](https://docsbot.ai/prompts/creative/ai-creative-director)  
14. JSON Prompting for AI Image Generation – A Complete Guide with Examples | ImagineArt, accessed December 18, 2025, [https://www.imagine.art/blogs/json-prompting-for-ai-image-generation](https://www.imagine.art/blogs/json-prompting-for-ai-image-generation)  
15. NANO BANANA PRO: Expert Use Cases with Prompts \- Higgsfield, accessed December 18, 2025, [https://higgsfield.ai/blog/Nano-Banana-Pro-Expert-Use-Cases](https://higgsfield.ai/blog/Nano-Banana-Pro-Expert-Use-Cases)  
16. Gemini 3 Pro Image API: Complete Developer Guide 2025 (Nano Banana Pro) \- Cursor IDE, accessed December 18, 2025, [https://www.cursor-ide.com/blog/gemini-3-pro-image-api](https://www.cursor-ide.com/blog/gemini-3-pro-image-api)  
17. The only prompting guide you need to master Bytedance's Seedance Pro: The best AI video model in 2025, accessed December 18, 2025, [https://www.atlabs.ai/blog/ultimate-seedance-1-pro-prompting-guide](https://www.atlabs.ai/blog/ultimate-seedance-1-pro-prompting-guide)  
18. Top 10 Viral Nano Banana Pro Prompts by Use Case: Transform Your Ideas with AI in 2025, accessed December 18, 2025, [https://www.atlabs.ai/blog/top-10-nano-banana-pro-prompts](https://www.atlabs.ai/blog/top-10-nano-banana-pro-prompts)  
19. The Best Nano Banana Prompts | metricsmule, accessed December 18, 2025, [https://metricsmule.com/ai/best-nano-banana-prompts/](https://metricsmule.com/ai/best-nano-banana-prompts/)  
20. How to Use the Nano Banana Pro(Gemini 3 Pro Image) API ? \- CometAPI \- All AI Models in One API, accessed December 18, 2025, [https://www.cometapi.com/how-to-use-the-nano-banana-pro-api/](https://www.cometapi.com/how-to-use-the-nano-banana-pro-api/)  
21. Google Antigravity: Inside Google's Agent-First Coding Platform | by Nalynelima \- Medium, accessed December 18, 2025, [https://medium.com/@nalynelima783/google-antigravity-inside-googles-agent-first-coding-platform-9c5696a25384](https://medium.com/@nalynelima783/google-antigravity-inside-googles-agent-first-coding-platform-9c5696a25384)  
22. Build with Nano Banana Pro, our Gemini 3 Pro Image model \- Google Blog, accessed December 18, 2025, [https://blog.google/technology/developers/gemini-3-pro-image-developers/](https://blog.google/technology/developers/gemini-3-pro-image-developers/)
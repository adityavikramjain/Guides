
# HTML Presentation JSON Schema Examples (Material Design 3 Optimized)

This document provides detailed examples of the JSON structure for various slide layouts, optimized for a modern HTML presentation using Material Design 3 components and icons. These examples illustrate how to construct the `content` array for different `layout` types and how to incorporate M3-style icons.

---

## JSON Structure Overview

```json
{
  "presentationTitle": "Your Presentation Title Here",
  "governedThought": "The single, powerful conclusion.",
  "audience": "Target Audience Description",
  "goal": "Persuade/Inform",
  "timeAllotted": "X minutes",
  "slides": [
    // Slide objects will go here
  ]
}
```

---

## Slide Layout Examples

### 1. `title_icon` Layout (Simple Title and Main Icon)

*   **Purpose:** Ideal for introductory slides, section breaks, or slides with a single, clear message.
*   **Visual:** Large title, prominent M3 icon, optional short paragraph.

```json
{
  "slideNumber": 1,
  "title": "Welcome: Architecting Clarity",
  "layout": "title_icon",
  "mainIcon": "design_services",
  "content": [
    { "type": "paragraph", "text": "Our journey to forge a powerful and persuasive presentation begins now." }
  ],
  "notes": "Greet the audience, set the stage, and introduce the presentation's purpose.",
  "cognitiveLoad": "Low"
}
```

### 2. `bullet_points` Layout (Title, Icon, and Key Bullet Points)

*   **Purpose:** Presenting lists, key takeaways, or sequential information.
*   **Visual:** Title, main icon, and a list of points, each optionally with its own small M3 icon.

```json
{
  "slideNumber": 5,
  "title": "Our Core Principles",
  "layout": "bullet_points",
  "mainIcon": "rule",
  "content": [
    { "type": "list_item", "text": "Governed Thought is King: One clear idea per presentation.", "icon": "diamond" },
    { "type": "list_item", "text": "Narrative Creates Desire: Move from 'What Is' to 'What Could Be'.", "icon": "spark" },
    { "type": "list_item", "text": "Clarity Through Restraint: High signal-to-noise ratio.", "icon": "lightbulb" },
    { "type": "list_item", "text": "Rhythm Creates Engagement: Balance complexity for audience energy.", "icon": "music_note" }
  ],
  "notes": "Elaborate on each principle, providing brief examples or context.",
  "cognitiveLoad": "Medium"
}
```

### 3. `two_column_icons` Layout (Side-by-Side Content with Icons)

*   **Purpose:** Comparing two ideas, presenting pros/cons, or showing related but distinct information.
*   **Visual:** Title, main icon, two distinct columns of content, each with its own heading, paragraphs, or bullet points, and optional M3 icons.

```json
{
  "slideNumber": 7,
  "title": "Current State vs. Future Vision",
  "layout": "two_column_icons",
  "mainIcon": "compare_arrows",
  "content": [
    { "type": "sub_heading", "text": "What Is (The Challenge)", "column": "left" },
    { "type": "paragraph", "text": "Our existing system faces significant performance bottlenecks.", "icon": "bug_report", "column": "left" },
    { "type": "list_item", "text": "Slow processing speeds.", "icon": "speed", "column": "left" },
    { "type": "list_item", "text": "High operational costs.", "icon": "money_off", "column": "left" },
    { "type": "sub_heading", "text": "What Could Be (The Solution)", "column": "right" },
    { "type": "paragraph", "text": "A new AI-driven platform will revolutionize our efficiency.", "icon": "rocket_launch", "column": "right" },
    { "type": "list_item", "text": "50% faster data processing.", "icon": "trending_up", "column": "right" },
    { "type": "list_item", "text": "30% reduction in costs.", "icon": "savings", "column": "right" }
  ],
  "notes": "Use this slide to create tension and highlight the contrast between problem and solution.",
  "cognitiveLoad": "High"
}
```

### 4. `image_caption` Layout (Main Image/Icon with Descriptive Text)

*   **Purpose:** When a single image or a dominant icon is the primary focus, with supporting text.
*   **Visual:** A large central icon or an image (if we ever support images directly), with a title and a descriptive paragraph.

```json
{
  "slideNumber": 9,
  "title": "The Power of Collaboration",
  "layout": "image_caption",
  "mainIcon": "diversity_3",
  "content": [
    { "type": "paragraph", "text": "Our success is built on the collective strength and diverse perspectives of our team members working together." }
  ],
  "notes": "Emphasize the importance of teamwork and how it contributes to achieving goals.",
  "cognitiveLoad": "Medium"
}
```

### 5. `section_header` Layout (For Section Transitions)

*   **Purpose:** To clearly delineate different sections of the presentation.
*   **Visual:** A large, simple title indicating the new section, often with a thematic icon.

```json
{
  "slideNumber": 10,
  "title": "Phase 2: Strategic Implementation",
  "layout": "section_header",
  "mainIcon": "flag",
  "content": [],
  "notes": "Signal a transition to a new major part of the presentation.",
  "cognitiveLoad": "Low"
}
```

### 6. `conclusion` Layout (Summary or Call to Action)

*   **Purpose:** Summarizing key points or presenting a clear call to action.
*   **Visual:** Prominent heading, main icon, and actionable items or summary points.

```json
{
  "slideNumber": 12,
  "title": "Your Next Step: Join the Movement",
  "layout": "conclusion",
  "mainIcon": "handshake",
  "content": [
    { "type": "heading", "text": "We ask you to:" },
    { "type": "list_item", "text": "Approve the Q3 budget for project Alpha.", "icon": "check_circle" },
    { "type": "list_item", "text": "Schedule a follow-up meeting by Friday.", "icon": "event" },
    { "type": "paragraph", "text": "Together, we can achieve unparalleled growth.", "icon": "trending_up" }
  ],
  "notes": "Reiterate the main call to action and inspire confidence.",
  "cognitiveLoad": "Medium"
}
These knowledge files will provide Maestro with a rich vocabulary of M3 icons and a clear understanding of how to structure the JSON for various slide types, aligning perfectly with your vision for a modern, icon-driven HTML presentation.

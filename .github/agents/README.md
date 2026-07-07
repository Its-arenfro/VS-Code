# Design Director Agent System

A comprehensive design critique system that helps teams make better design decisions through specialized expert agents.

## Overview

The Design Director orchestrates specialized agents to provide expert feedback across multiple design domains. Instead of getting generic feedback, you get focused, domain-specific critique from agents trained on:

- **Accessibility** — WCAG compliance & inclusive design
- **Heuristics** — Usability principles & design patterns
- **Research** — Design trends & best practices
- **UI Design** — Visual design & layout
- **Copywriting** — Brand voice & messaging
- **Design-Thinking** — User empathy & problem reframing

## Getting Started

### 1. Open Copilot Chat
In VS Code, open Copilot Chat (Cmd+Shift+L or click the Copilot icon).

### 2. Invoke the Design Director
Type `/Design Director` and press Enter.

### 3. Share Your Design
Paste a screenshot, Figma link, or description of what you're working on.

### 4. Choose Your Reviews
The Design Director will ask which aspects matter most to you. Select one or more:
- Just accessibility? ✓
- Full review (all agents)? ✓
- Specific focus (UI + copy)? ✓

### 5. Get Feedback
The Director deploys your chosen agents and synthesizes their findings into actionable recommendations.

## Available Agents

### Design Director (Main Orchestrator)
**When to use:** You want comprehensive design feedback

**What it does:**
- Understands your design context
- Asks which review aspects you want
- Deploys the right specialist agents
- Synthesizes findings into priorities
- Suggests next steps

### Accessibility Agent
**When to use:** Ensuring WCAG compliance and inclusive design

**Covers:**
- Color contrast (WCAG AA minimum)
- Keyboard navigation
- Focus indicators
- Alt text & labels
- Motion & animations
- Touch targets (mobile)
- Assistive tech compatibility

### Heuristics Agent
**When to use:** Evaluating usability and design patterns

**Covers:**
- Nielsen's 10 Usability Heuristics
- Error prevention & recovery
- User control & freedom
- Consistency & standards
- System feedback & visibility
- Flexibility for power users

### Research Agent
**When to use:** Grounding decisions in design patterns and trends

**Covers:**
- Industry best practices
- Competitive benchmarks
- Design patterns & conventions
- User research insights
- Case studies & examples
- Relevant guidelines (iOS, Android, web)

### UI Design Agent
**When to use:** Refining visual design and layout

**Covers:**
- Visual hierarchy & contrast
- Typography & readability
- Layout & composition
- Spacing & alignment
- Color theory & palette
- Interactive states
- Responsive behavior

### Copywriter Agent
**When to use:** Polishing messaging and brand voice

**Covers:**
- Brand voice consistency
- Microcopy (buttons, labels, errors)
- Clarity & simplicity
- Error messaging
- Confirmation messages
- Terminology consistency

### Design-Thinking Agent
**When to use:** Exploring user needs and alternative solutions

**Covers:**
- User empathy & context
- Problem reframing
- Assumption challenging
- Journey mapping
- Emotional touchpoints
- Alternative solutions

## Workflow Examples

### Example 1: Quick Accessibility Check
```
1. Invoke: /Design Director
2. Share: Screenshot of new form
3. Choose: Accessibility only
Result: Specific WCAG issues + fixes
```

### Example 2: Full Design Review
```
1. Invoke: /Design Director
2. Share: Figma link to new feature
3. Choose: All agents
Result: Comprehensive critique across all domains, prioritized
```

### Example 3: User-Centered Redesign
```
1. Invoke: /Design Director
2. Share: Current design + user feedback
3. Choose: Design-Thinking + Heuristics
Result: Alternative approaches + usability improvements
```

## Tips for Best Results

### 1. Provide Context
- **What** are you designing? (Feature, page, component)
- **Who** is it for? (User type, use case)
- **Why** does it matter? (Business goal, problem solving)
- **Constraints?** (Brand guidelines, technical limits, timeline)

More context = more targeted feedback.

### 2. Be Specific
Instead of: "Review this design"
Try: "We're redesigning checkout for mobile users. Main goal is reducing cart abandonment. Can you check accessibility and heuristics?"

### 3. Iterate
Use feedback from one review to inform the next iteration. The agents can help you refine solutions.

### 4. Choose Strategically
- **Early stage?** Design-Thinking + Research = explore the problem
- **Middle stage?** Heuristics + UI Design = refine the solution
- **Late stage?** Accessibility + Copy = polish & compliance

### 5. Screenshot Best Practices
- If sharing screenshots: Make them clear and in context (full page when possible)
- If sharing Figma: Use link format so agents can see current state
- Include viewport context (desktop/mobile/tablet)

## For Team Leads

### Sharing Designs with Reviews
When presenting a design to the team:
1. Get Design Director feedback first
2. Share findings alongside the design
3. Use agents' structured feedback for design critique meetings

### Standardizing Design Quality
Use the Design Director as a baseline review before design handoff:
- Accessibility check (before dev)
- Heuristics review (before launch)
- Copy review (before user-facing)

### Onboarding New Designers
Have them use the Design Director to learn design principles through feedback on their work.

## Customizing Agents

Each agent is defined in a separate `.agent.md` file:
- `design-director.agent.md` — Main orchestrator
- `accessibility.agent.md` — Accessibility specialist
- `heuristics.agent.md` — Usability expert
- `research.agent.md` — Design researcher
- `ui-design.agent.md` — Visual designer
- `copywriter.agent.md` — Copy specialist
- `design-thinking.agent.md` — User experience strategist

To customize an agent's behavior, edit the corresponding `.agent.md` file and commit changes to git.

## Limitations & Considerations

- **Screenshots only for visual review** — Agents analyze what you show them
- **No real testing** — Agents provide feedback, but user testing is still essential
- **Context matters** — The better your context, the better the feedback
- **Not a replacement for expertise** — Use as a tool to enhance human judgment, not replace it

## Feedback & Improvements

Found an issue or have an improvement idea?
- Create an issue in the repo
- Suggest improvements to agent instructions
- Share examples of great/poor feedback

## Questions?

See any agent's `.agent.md` file for detailed domain coverage and methodology.

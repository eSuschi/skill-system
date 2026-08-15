# Pipeline Stages – Detailed

## 1. Requirements Clarifier
**Goal:** Eliminate ambiguity and missing information before any real work starts.

Key questions that must be answered:
- What exactly is being built and for whom?
- What is the primary success criterion?
- What is explicitly out of scope?
- What constraints exist (time, tech, platform, quality level)?
- What does "done" look like?

Output: Clear, written brief that both sides agree on.

## 2. Product Impact Architect
**Goal:** Decide if the project is worth building and define the highest-leverage approach.

Focus:
- Real user / business impact
- Differentiation from existing solutions
- First-principles evaluation
- Scope that maximises value vs effort

Output: Go / No-go + recommended shape of the solution.

## 3. Domain Specialist Execution
**Goal:** High-quality implementation by the most appropriate specialist skill(s).

Examples of specialists:
- Advanced Website Expert / Business Site Studio
- Principal Engine Architect
- Browser Game Expert
- AI Meeting Buddy Builder
- Senior Software Engineer
- Principal Life App Architect

Output: Working code + documentation that meets professional standards.

## 4. Principal Code Review
**Goal:** Deep technical review focused on correctness and long-term quality.

Looks for:
- Logic errors and edge cases
- Race conditions and resource leaks
- API / contract stability
- Error handling
- Maintainability and clarity

## 5. Final Code Auditor
**Goal:** Full-system quality scan before release consideration.

Checks:
- Functionality (does it actually work?)
- Visual / UX polish
- Language consistency
- Missing edge cases
- Security basics
- Overall usefulness

## 6. Release Gate
**Goal:** Final mandatory barrier. Nothing ships with Critical or High defects.

Criteria:
- All previous stages passed
- Product is genuinely usable
- Looks and feels professional
- No known Critical/High issues
- Ready to show the world

# Deep Background Verification Prompt (Starter Version)

## Purpose
This is a simplified version of the full Deep Background prompting system for business leaders who need to quickly verify claims, check sources, and identify hidden caveats in proposals, reports, or strategic recommendations.

For the complete system with all features, see [deep_background.md](../research/deep_background.md)

## How to Use

1. Copy the prompt below
2. Paste it into ChatGPT, Claude, or your preferred AI assistant (Search enabled tools are best)
3. After the prompt, provide the claim or content you want to verify
4. Review the structured output to make informed decisions

---

## The Prompt

```
You are a fact-checking and verification assistant. When I provide you with a claim, statement, or content to analyze, follow this process:

1. IDENTIFY THE CLAIM
   - State what the core claim is
   - Identify what the claim is supposed to be evidence FOR
   - Note both a moderate and strong version of what's being argued

2. VERIFY FACTS
   Create a table with these columns: Statement | Status | Evidence & Source | Confidence (1-5)
   - Mark verified facts as ✅ Correct
   - Provide specific evidence with source links
   - Rate confidence level for each verification

3. IDENTIFY ERRORS OR CAVEATS
   Create a table with these columns: Statement | Issue | Correction | Confidence (1-5)
   - Mark factual errors as ❌ Incorrect
   - Mark unsubstantiated claims as ❓ Unable to verify
   - Provide corrections with specific evidence
   - Note important caveats that change the meaning

4. ASSESS SOURCES
   Create a table: Source | Usefulness | Notes | Rating (1-5)
   - Evaluate the credibility of sources cited
   - Note any potential biases or conflicts of interest
   - Identify what's missing (e.g., "No independent verification")

5. PROVIDE REVISED SUMMARY
   Write a 2-3 paragraph corrected version that:
   - Integrates verified facts
   - Includes discovered caveats
   - Corrects errors or misleading framing
   - Maintains neutrality while being accurate

6. KEY TAKEAWAYS
   List 3-5 bullet points of what decision-makers need to know:
   - What's actually true vs. what was claimed
   - Important caveats or conditions
   - What additional verification is needed
   - Red flags or areas of concern

IMPORTANT:
- All links must be actual, working URLs—no placeholder or search links
- Rate source credibility honestly (1=unreliable, 5=highly reliable)
- Acknowledge when you cannot verify something
- Flag when claims lack specifics (no dates, places, or reference to specific studies)
- Note when "averages" or aggregates might hide important variation

Now, please analyze the following:
```

---

## Example Usage

**Your Input:**
```
[Paste the prompt above]

Now analyze this claim:

"Our AI platform has helped enterprise clients reduce customer service costs by 40%
while improving customer satisfaction scores by 25%. Implementation takes just 8 weeks."
```

**What You'll Get:**
- Table showing which parts are verifiable vs. questionable
- Source analysis (are these verified case studies or marketing claims?)
- Caveats discovered (e.g., "40% reduction only for tier-1 tickets", "8 weeks assumes existing data infrastructure")
- Revised summary with the complete, accurate picture
- Key takeaways for decision-making

---

## Tips for Best Results

1. **Be Specific**: Provide the exact claim, including context about who made it and when
2. **Include Sources if Available**: If the claim cites studies or case studies, include those references
3. **Ask Follow-ups**: Use "Do another round focusing on [specific aspect]" to dig deeper
4. **Check the Checkers**: If the AI cites sources, click them to verify they're real and relevant
5. **Focus on What Matters**: Ask specifically about the claims that would influence your decision

---

## Common Use Cases

- **Vendor Proposals**: Verify performance claims, case studies, and implementation timelines
- **Strategic Reports**: Check the data and assumptions underlying recommendations
- **Market Research**: Verify statistics, trends, and competitive claims
- **Due Diligence**: Systematically verify claims about companies you're considering partnering with or acquiring

---

## When to Use the Full System

This starter version is great for quick verification. Use the [full deep_background.md](./deep_background.md) system when you need:
- Image verification and provenance checking
- Toulmin argument analysis
- Discourse mapping showing competing viewpoints
- Deep investigation with multiple rounds of research
- Academic-level rigor with comprehensive source tables


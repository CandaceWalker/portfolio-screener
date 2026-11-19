# Portfolio Screener 🎨

An AI agent that helps recruiters screen design and creative portfolios against a role-specific rubric. It narrows the pool so people can spend their time on the strongest candidates. **The agent never rejects anyone. People make every hiring decision.**

Works with a **Claude Project** or a **Gemini Gem**. No code required.

## Why I built it
A single design opening can bring in hundreds of portfolios. Reviewing them well takes time, and staying consistent across all of them is hard. Using this approach, I took one Visual Design search from **250 applicants to 20 finalists** and cut screening time by about **60%**.

## How it works
1. You define what "great" looks like for the role in a short rubric.
2. The agent scores each portfolio against that rubric, citing specific work as evidence.
3. It sorts candidates into tiers so you know who to review first:

| Tier | Meaning |
|---|---|
| **A** | Strong match. Review first. |
| **B** | Promising, with a specific gap or question. |
| **C** | Not a match for this role based on the portfolio. |
| **Needs human review** | The agent couldn't see enough of the work to judge fairly. |

## Built-in fairness rules
- Evaluates the **work**, not the person. Ignores names, photos, schools, age, and personal details.
- Never infers or mentions protected characteristics.
- Doesn't penalize career gaps or non-traditional backgrounds.
- Uses tiers instead of rejections, so a human always makes the call.

## Files
| File | What it's for |
|---|---|
| [`agent-instructions.md`](agent-instructions.md) | Paste once into your Claude Project or Gemini Gem |
| [`rubric-template.md`](rubric-template.md) | Fill in for each new role |
| [`example-rubric-visual-designer.md`](example-rubric-visual-designer.md) | A filled-in example |

## Setup
1. Create a **Claude Project** or **Gemini Gem**.
2. Paste the contents of `agent-instructions.md` into its instructions.
3. For each role, fill in `rubric-template.md` with the hiring manager and send it as your first message.
4. Send portfolios in batches of 10–20, using candidate IDs or initials instead of full names.

## Tips
- **Calibrate first.** Run 5–10 portfolios you've already reviewed and check that the agent agrees with you. Adjust the rubric if it doesn't.
- **Spot-check Tier C** in every batch so strong candidates don't slip through.
- **The rubric is everything.** Vague criteria produce vague results.

## Before using with real candidates
- Check your company's policy on AI tools and candidate data.
- Some places regulate automated tools in hiring (for example, New York City and California). Keeping a human decision-maker helps, but confirm with your legal or HR team.
- Share only what the screen needs, and remove personal details where you can.

---

📫 [Connect with me on LinkedIn](https://linkedin.com/in/candacerwalker)

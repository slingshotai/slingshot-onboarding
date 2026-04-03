# Module 6: Supercharge SAM's Brain

## What We're Doing

In Module 2, SAM was installed with a starter brain — enough to teach the Slingshot Framework basics and answer general questions. Now that you've authenticated GitHub (Module 5), we can give SAM the full knowledge base.

This upgrades SAM from "knows the overview" to "knows every framework detail, every playbook, every methodology deep-dive." It's the difference between a mentor who's read the summary and one who wrote the book.

## What's in the Full Brain?

SAM's brain has two sections:

### Framework Knowledge
The complete Slingshot Framework with deep-dives into each area:
- **Sell** — Product Quadrant, hero product strategy, demand analysis
- **Story** — The Story Overlap, brand messaging, the We vs You diagnostic
- **Tech Stack** — platform strategy, mobile-first architecture
- **Marketing** — the full FUEL framework (Foundation → Unlock → Elevate → Leapfrog) across all 8 marketing areas
- **Optimise** — conversion pillars, product page methodology, CTA strategy
- **Experience** — post-purchase journey, unboxing, onboarding sequences
- **Growth** — the three growth variables, referral systems, loyalty

### Playbooks
Research-backed playbooks on specific topics:
- Viral coefficient and referral-driven growth
- Paid membership programme design
- More added regularly as new research is completed

## Install the Full Brain

This is a one-prompt job. Ask Claude:

```
Clone SAM's brain from https://github.com/slingshotai/sam-brain and install it.
Put the brain folder at ~/.claude/skills/sam/brain/
```

Claude will:
1. Clone the private repo (works because you authenticated GitHub in Module 5)
2. Copy the brain folder to SAM's skill directory
3. Confirm what was installed

## Test It

Ask SAM something that needs deep framework knowledge:

```
sam, explain the Story Overlap and how I can use it on my site
```

With the starter brain, SAM would give you the basics. With the full brain, SAM walks you through the complete methodology — the Venn diagram, the We vs You ratio diagnostic, the three-step process for finding your overlap, the Netflix headline formula, and specific examples you can apply to your business.

Try another:

```
sam, walk me through the FUEL matrix for my marketing
```

SAM now has the full 4x8 matrix — every marketing area at every FUEL stage — and can assess where your business sits across all 32 combinations.

## What Just Changed

SAM went from knowing the headlines to knowing the full methodology. Every question you ask now draws from the same knowledge base that powers SlingshotAI's paid skills. This is Matt's 20+ years of ecommerce experience, structured and searchable.

And it keeps growing. As new framework content and playbooks are added, you update with:

```
sam, update brain from https://github.com/slingshotai/sam-brain
```

## Keeping the Brain Updated

The brain updates separately from SAM itself:
- `sam, update` — checks the main SAM repo for skill updates
- `sam, update brain from https://github.com/slingshotai/sam-brain` — checks the brain repo for new knowledge

We'll let you know when significant brain updates ship — new framework areas, new playbooks, refined methodology.

---

[[05 - Install Your First Skill|← Install Your First Skill]] | [[07 - The Slingshot Framework|Next → The Slingshot Framework]]

# Bonus Module: Create Your Own Skill

## What We're Doing

You've learned how to install and run skills. Now you're going to learn how to build one.

This is optional — not everyone will want to create their own skills. But if you're the kind of founder who builds systems, who creates SOPs, who documents "how we do things" — this module turns that instinct into something Claude can execute automatically.

By the end of this module, you'll understand how to:
- Write a SKILL.md file
- Structure a skill with references and learning content
- Use Anthropic's official skill-creator to test and improve your skill
- Install and run your own creation

## Why Build Your Own Skills?

Every business has processes that are repeated but never documented. Things like:

- How you write product descriptions for your store
- How you respond to specific types of customer complaints
- How you evaluate a new supplier
- How you brief a freelancer
- How you prepare for a quarterly review

Right now, these processes live in your head (or your team's heads). A skill takes that knowledge and makes it executable — Claude follows the process the same way every time, with the quality bar you've set.

Think of it this way: every SOP you've ever written could become a skill. Except instead of someone reading the SOP and trying to follow it, Claude reads it and does it.

## The Anatomy of a Simple Skill

At its most basic, a skill is a single file:

```markdown
---
name: my-skill-name
description: "What this skill does and when to use it."
user-invocable: true
---

# My Skill

Instructions for Claude go here.

## Steps

1. Do this first
2. Then do this
3. Finally, produce this output
```

That's a working skill. Save it as `SKILL.md` in `~/.claude/skills/my-skill-name/` and Claude can run it immediately.

## The Anthropic Skill Creator

Anthropic — the company behind Claude — has built an official tool for creating and testing skills. It's called the skill-creator, and it handles:

- **Test cases** — define prompts that should trigger your skill and check the outputs
- **Evaluation** — run your skill against test cases and review the results
- **Description optimisation** — automatically refine your skill's description so it triggers correctly
- **Benchmarking** — compare your skill with and without changes

### Installing the Skill Creator

Ask Claude:

```
Install the Anthropic skill-creator plugin. I want to create and test my own skills.
```

Claude will set it up. Once installed, you can use `/skill-creator` to access its full workflow.

## Your First Skill: A Quick Win

Let's build something simple and useful. Pick a task you do regularly — something that follows a repeatable pattern.

**Example: A product listing checker**

```
Help me create a skill called "listing-check" that:
1. Takes a product page URL
2. Checks if the title, description, images, and price are present
3. Flags anything missing
4. Produces a simple checklist showing what's done and what needs attention
Save it as a SKILL.md I can install.
```

Claude will write the SKILL.md for you. Review it, adjust anything that doesn't match your process, and install it.

### Test It

```
/listing-check https://your-store.com/products/your-product
```

If it works — congratulations, you've built a skill. If it doesn't quite produce what you want, iterate: "The checklist should also check for alt text on images" or "Add a section that checks the meta description."

## Making It Better: The Skill Creator Workflow

Once you have a working draft, the skill-creator helps you refine it:

1. **Create test cases** — real prompts a user would type to trigger your skill
2. **Run the tests** — see how your skill performs on each one
3. **Review outputs** — check if the quality is where you want it
4. **Iterate** — improve the SKILL.md based on what you see
5. **Optimise the description** — make sure Claude triggers your skill at the right times

This is the same process we use to build every SlingshotAI skill. The tools are the same — the difference is the methodology and experience that goes into ours.

## Adding Learning Content for SAM

If you want SAM to be able to teach from your skill, add a `learn/` folder:

```
my-skill/
├── SKILL.md
└── learn/
    ├── overview.md       # What the skill does and why
    ├── methodology.md    # How it works in detail
    └── faq.md            # Common questions
```

Each file needs frontmatter with `skill`, `topic`, and `keywords` fields so SAM can find it. Look at any SlingshotAI skill's learn folder for the format.

## Ideas for Skills You Could Build

| Task | Skill idea |
|---|---|
| Writing product descriptions | A skill that follows your specific formula with your brand voice |
| Responding to reviews | A skill that drafts responses in your tone, handling positive and negative |
| Weekly reporting | A skill that pulls together key metrics and writes a summary |
| Supplier evaluation | A skill that scores a potential supplier against your criteria |
| Content briefs | A skill that creates a brief for a freelancer using your standards |
| Customer segmentation | A skill that categorises customer enquiries by type |

The pattern: if you've ever written an SOP, a checklist, or a "how we do this" document — that's a skill waiting to be built.

## The SlingshotAI Skill Creation Skill

If you want to go deeper, there's a dedicated skill in the SlingshotAI store that teaches the full skill-building methodology — not just the technical "how to write a SKILL.md" but the strategic thinking behind what makes a great skill: when to use references, how to structure scoring rubrics, how to write descriptions that trigger correctly, and how to build learn/ content that SAM can teach from.

It's essentially a meta-skill — a skill that teaches you to build skills.

---

[[08 - Whats Next|← What's Next]]

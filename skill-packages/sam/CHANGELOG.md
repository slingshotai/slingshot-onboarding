# SAM — Changelog

## v1.1.0 — 2026-04-03

Major architecture update.

- **Three knowledge layers**: Brain (Matt's direct knowledge), EP Knowledge (podcast evidence), Skill learn/ folders. Search priority: brain → skills → EP → research.
- **Starter brain**: Framework overviews ship with the public SAM repo. Full brain cloned separately from private `sam-brain` repo in Module 6.
- **Full update system**: `sam, update` now checks ALL components — SAM skill, brain, EP Knowledge, EP Weekly Brief, and all purchased skills. Presents a summary table with version comparisons and changelogs.
- **Update mode**: Added to mode table. Triggered by "sam, update", "check for updates", "new version".
- **Repo renamed**: `slingshot-onboarding` → `sam`. Old URLs redirect automatically.
- **Course restructured**: New Module 6 (Supercharge SAM's Brain), renumbered 07-10. Story Overlap moved to brain. Bonus module removed.
- **Video-vs-prompt notes**: Modules 1-4 now note that written prompts may differ from video versions.

## v1.0.0 — 2026-04-03

Initial release.

- SAM core: Q&A, Guided Lesson, Demo, and Discovery modes
- Voice guide: Matt Edmundson's teaching voice
- Member profile system (`~/.slingshot/profile.md`)
- Multi-site support with currency localisation
- Slingshot Framework learn content (7 areas, FUEL, Product Quadrant, Story Overlap)
- Cross-skill routing: searches all installed skills' `learn/` folders
- Custom overrides: `custom/` folder preserved across updates
- Version tracking: `version` field in frontmatter + this changelog

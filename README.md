# LinkedIn Post Generator Skill

A reusable Hermes Agent skill for writing LinkedIn posts that are specific, human, credible, and useful without sounding like generic AI-generated content.

## What it covers

- Personal learning posts
- Opinion and contrarian posts
- Technical explanations for non-technical audiences
- Project breakdowns
- Product and feature announcements
- Build-in-public updates
- Service and agency positioning
- Critical reviews
- Hook generation
- Content repurposing
- Carousel and visual direction

This public version focuses on LinkedIn content. Recruiter outreach, cover letters, and job-application writing are intentionally outside its scope.

## Privacy-safe customization

The skill uses generic guidance by default. To configure it for a recurring personal or company voice:

```bash
cp PROFILE_TEMPLATE.md PROFILE.md
```

Fill in the values in `PROFILE.md`, then keep that file private. It is ignored by Git through `.gitignore`.

The profile supports variables such as:

- `{{AUTHOR_NAME}}`
- `{{ACCOUNT_TYPE}}`
- `{{COMPANY_NAME}}`
- `{{COMPANY_POSITIONING}}`
- `{{AUTHOR_BACKGROUND}}`
- `{{TARGET_AUDIENCE}}`
- `{{PRODUCT_OR_SERVICE}}`
- `{{VOICE_TRAITS}}`
- `{{TONE_PREFERENCES}}`
- `{{CTA_PREFERENCE}}`
- `{{LINKEDIN_URL}}`

Do not put passwords, API keys, private client information, or confidential company strategy in the profile.

## Installation

Clone the repository somewhere safe first:

```bash
git clone https://github.com/zh10only1/linkedin-post-generator-skill.git
```

To install it as a Hermes skill without overwriting an existing skill, copy the directory into your Hermes skills folder under a distinct name or back up the existing directory first:

```bash
mkdir -p ~/.hermes/skills/social-media
cp -R linkedin-post-generator-skill ~/.hermes/skills/social-media/linkedin-post-generator
```

If you already have a personalized skill at that path, do not run the copy command until you have backed it up or chosen another directory.

## Files

```text
SKILL.md
PROFILE_TEMPLATE.md
README.md
LICENSE
CHANGELOG.md
```

The repository intentionally contains no post-specific reference files. Add examples locally if you need them for a particular project or brand.

## Design principles

- Real voice over polished writing
- Specificity over vague inspiration
- Point of view over generic advice
- Credibility over hype
- Useful engagement over engagement bait
- No invented metrics, experiences, clients, or results
- No unresolved template variables in final posts

## License

MIT. See `LICENSE`.

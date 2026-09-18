---
name: linkedin-post-generator
description: Generate, improve, and critique LinkedIn posts that sound human, specific, opinionated, and useful. Use when users request LinkedIn posts, professional social content, founder posts, product updates, thought leadership, project breakdowns, or rewrites of business-related content.
metadata:
  version: 1.0.0
  authoring_notes: Public, reusable version with profile placeholders and privacy-safe references.
---

# LinkedIn Post Generator

## Overview

This skill helps create LinkedIn posts that sound like a real person with a real point of view, not generic AI-written business content.

The goal is not just to produce a clean post. The goal is to produce a post that has:

- A clear reason to exist
- A specific audience
- A sharp angle or useful takeaway
- Natural human language
- The user's actual voice
- Enough specificity to feel credible
- No fake numbers, fake stories, fake client results, or manufactured emotion

Use this skill whenever the user wants to:

- Create a LinkedIn post from an idea, rough note, rant, project, or experience
- Rewrite a LinkedIn post to make it sharper, more human, or less generic
- Turn technical work into a founder-friendly or client-friendly post
- Create company updates without corporate fluff
- Share project learnings, opinions, product updates, lessons, or behind-the-scenes thinking
- Build thought leadership without sounding like a content farm
- Review an existing post and identify what is weak
- Generate multiple post angles from the same topic

## Customization Profile

This public version is designed to be reusable across personal and company LinkedIn accounts.

Before using it for a recurring voice, copy `PROFILE_TEMPLATE.md` to a local `PROFILE.md` in the same skill directory and replace the template values. Keep `PROFILE.md` private and do not commit it to a public repository.

The profile may contain values such as:

- `{{AUTHOR_NAME}}`: the person whose voice is being represented
- `{{ACCOUNT_TYPE}}`: `personal` or `company`
- `{{COMPANY_NAME}}`: the company or brand name, if applicable
- `{{COMPANY_POSITIONING}}`: how the company wants to be understood
- `{{AUTHOR_BACKGROUND}}`: relevant experience or perspective
- `{{TARGET_AUDIENCE}}`: the primary audience for the post
- `{{PRODUCT_OR_SERVICE}}`: the product, service, or subject being discussed
- `{{VOICE_TRAITS}}`: desired voice characteristics
- `{{TONE_PREFERENCES}}`: preferred tone and level of directness
- `{{CTA_PREFERENCE}}`: preferred ending or call-to-action style
- `{{LINKEDIN_URL}}`: relevant profile or company-page URL

If `PROFILE.md` is not available, use only information supplied in the current request. Do not guess profile values, company details, achievements, metrics, or personal experiences. Ask for a missing value only when it materially affects the post.

Never copy unresolved template variables into a final post. Replace them with verified information, remove them, or rewrite around them.

## Core Philosophy

A good LinkedIn post should feel like a smart conversation with someone you respect.

It should not feel like:

- A press release
- A motivational quote
- A generic AI essay
- A fake founder story
- A sales pitch pretending to be advice
- A neat lesson wrapped around a story that probably never happened

The best posts usually do one of these things:

- Say something specific that others are thinking but not saying clearly
- Challenge a common assumption
- Share a real lesson from actual work
- Explain a technical or business idea in simple language
- Show how the writer thinks
- Give readers a useful lens they can apply

## Default Style

Unless the user provides another preference, write in this style:

- Professional but conversational
- Direct, practical, and grounded
- Slightly informal when natural
- No corporate clichés
- No excessive inspiration
- No exaggerated claims
- No em dashes
- No forced hype
- No fake vulnerability
- Short paragraphs with clean spacing
- Clear but not over-polished

The voice should feel like someone explaining an idea to a smart colleague, founder, client, or peer.

## Operating Rule

Do not blindly generate a post from the topic.

First, identify the underlying idea.

Before writing, silently determine:

1. What is the real point?
2. Who is this for?
3. Why should they care?
4. What is the tension, mistake, belief, or lesson?
5. What specific context is available?
6. What must not be invented?
7. What tone best matches the user's intent?

Only ask clarifying questions if missing information would materially change the output.

If the user gives enough context, do not slow them down with questions. Make reasonable assumptions and produce a useful first version.

## Do Not Invent Details

This is a strict rule.

Never invent:

- Revenue
- Growth numbers
- Time saved
- Percentages
- User counts
- Client names
- Company names
- Testimonials
- Product results
- Deadlines
- Internal team details
- Personal experiences
- Emotional reactions
- Quotes from people

If a useful detail is missing, either:

- Use a placeholder like `[specific result]`
- Ask one focused question
- Rewrite without needing that detail

Bad:

> We reduced onboarding time by 40%.

Better:

> The goal was simple: reduce the amount of manual work users had to do before getting value from the product.

Better with placeholder:

> We reduced onboarding time by [specific result], but the more important lesson was what we removed, not what we added.

## Voice Capture

When the user provides an existing draft, rough note, caption, or past writing sample, preserve their voice unless they explicitly ask for a different tone.

Look for:

- Sentence length
- Casual phrases
- Level of bluntness
- Use of first person
- Humor or sarcasm
- Technical depth
- Confidence level
- How polished or raw the writing feels
- Words they use often
- Words they avoid

Do not over-sanitize the user's personality.

If the user's rough idea is casual, keep it casual.
If the user's idea is critical, keep the edge.
If the user's idea is technical, simplify without dumbing it down.
If the user's idea is uncertain, do not make it sound falsely confident.

### Voice Calibration Questions

Ask these only when useful:

- Should this sound more personal, more founder-like, or more educational?
- Should the take be soft and balanced, or sharper and more opinionated?
- Who exactly is this for?
- Do you want this to attract clients, start discussion, or just share a learning?
- Is there a specific example, metric, or project detail I should include?

## POV Extraction

Most weak LinkedIn posts fail because they do not have a point of view.

Before drafting, identify the post's POV.

A strong POV usually fits one of these patterns:

- People think X, but in practice Y happens.
- The real problem is not X, it is Y.
- We keep optimizing the wrong thing.
- This common advice is incomplete.
- This tool/process/trend is useful, but only under certain conditions.
- The boring part of the work matters more than the shiny part.
- The mistake was not technical, it was strategic.
- The lesson is obvious in hindsight, but easy to ignore while building.

Do not use these patterns mechanically. Use them to find the real angle.

### Weak POV Examples

Weak:

> AI can help teams become more productive.

Stronger:

> A lot of teams are not becoming AI-forward. They are becoming AI-anxious. They are adding AI to workflows before asking whether that workflow even needed AI.

Weak:

> Good communication is important in projects.

Stronger:

> Most project delays I have seen were not caused by bad code. They were caused by unclear decisions that everyone assumed someone else had made.

Weak:

> We should build user-friendly products.

Stronger:

> A feature is not user-friendly just because it is easy to click. It is user-friendly when the user does not have to understand your internal logic to use it.

## Audience Positioning

Always write for a specific audience, even if the user does not explicitly state one.

Possible audiences:

- Founders
- Technical founders
- Non-technical founders
- Agency owners
- Developers
- Product managers
- Designers
- Startup teams
- B2B service buyers
- Clients
- Peers in tech
- Operators and managers

Before writing, infer:

- What does this audience already care about?
- What misconception might they have?
- What pain are they dealing with?
- What would make them stop scrolling?
- What would make them comment or save the post?

Do not write for everyone. Posts written for everyone usually feel vague.

## Content Modes

Choose the best mode based on the user's goal.

### 1. Personal Learning Post

Use when the user shares a mistake, realization, project challenge, or lesson.

Structure:

1. Start with the moment, mistake, or realization
2. Give brief context
3. Explain what changed in your thinking
4. Share the lesson
5. Connect it to the reader's work
6. End with a grounded question or closing line

Avoid fake drama. Keep it real.

### 2. Opinion or Contrarian Post

Use when the user has a take on a trend, industry behavior, AI, startups, product, engineering, or work culture.

Structure:

1. Lead with the take
2. Explain why the common view is incomplete
3. Add a real example or practical reasoning
4. Include nuance so it does not sound like rage bait
5. End with a useful takeaway or discussion prompt

The post should be sharp, not arrogant.

### 3. Technical Insight Post

Use when the user wants to explain technical work in a way that non-technical people can understand.

Structure:

1. Lead with the business or user problem
2. Explain the technical idea in simple terms
3. Show the practical tradeoff
4. Mention what the user learned
5. Keep jargon minimal

Do not turn it into a tutorial unless requested.

### 4. Project Breakdown Post

Use when the user wants to talk about a completed project, client work, product build, or implementation.

Structure:

1. Lead with what was built or solved
2. Explain the problem behind it
3. Mention the stack or process only if relevant
4. Share the hardest or most interesting part
5. Explain the outcome without inventing metrics
6. End with a lesson or reflection

This should not read like a resume bullet list.

### 5. Product or Feature Launch Post

Use when announcing a launch, feature, update, or new capability.

Structure:

1. Lead with the problem solved
2. Explain what is now possible
3. Give brief context on why it was built
4. Mention who it is for
5. Include link or CTA if provided
6. End with a simple invitation

Avoid:

- Excited to announce
- Thrilled to share
- Game-changer
- Revolutionary
- We are proud to unveil

### 6. Build-in-Public Update

Use when sharing progress, experiments, decisions, pivots, or behind-the-scenes work.

Structure:

1. State what changed or what was learned
2. Explain what prompted the change
3. Share the tradeoff or decision
4. Mention what comes next if relevant
5. Invite useful feedback

Keep it honest. Do not exaggerate progress.

### 7. Service or Agency Post

Use when the user wants to attract clients without sounding salesy.

Structure:

1. Lead with a client problem or market observation
2. Explain why it matters
3. Share how the service solves or reduces that pain
4. Show credibility through process, not hype
5. End with a soft CTA if appropriate

Avoid direct hard-selling unless the user asks for it.

### 8. Review or Critique Post

Use when the user wants to critique a trend, workflow, tool, industry habit, or common mistake.

Structure:

1. Open with the issue
2. Explain why it happens
3. Show the hidden cost
4. Add nuance
5. Suggest a better way to think about it

Be critical without sounding bitter.

## Hook Rules

The hook should make the reader want to continue.

Good hooks usually create one of these:

- Tension
- Curiosity
- Specificity
- A clear opinion
- A relatable work problem
- A surprising framing

### Good Hook Examples

- The problem was not the AI feature. The problem was that nobody asked whether the workflow needed AI in the first place.
- A lot of startup advice sounds useful until you actually have to implement it with a real team and a real deadline.
- The more I work on products, the more I realize bad UX is often just exposed internal complexity.
- Most technical debt does not start as laziness. It starts as a reasonable shortcut that nobody revisits.
- We spent too much time asking what to build and not enough time asking what to remove.

### Weak Hook Examples

- I wanted to share some thoughts about AI.
- Here are 5 lessons I learned.
- In today's fast-paced world...
- Excited to announce...
- Productivity is very important.

## AI-Slop Avoidance

Avoid patterns that make posts feel generic or obviously AI-generated.

Do not overuse:

- Most people think X, but actually Y
- Here is what nobody tells you about X
- X is not about Y. It is about Z
- I used to think X. Now I think Y
- Let that sink in
- Read that again
- The truth is...
- In today's fast-paced world
- The future of work is...
- This changed everything
- This is a game-changer
- Here are 5 lessons from X
- A vague story followed by a perfect lesson

These structures are not banned entirely, but they should only be used if they genuinely fit the idea.

A post should not feel like it came from a template.

## Language Rules

Use:

- Simple words
- Short paragraphs
- Specific examples
- Concrete nouns
- Natural transitions
- First person when appropriate
- Active voice
- Controlled confidence

Avoid:

- Corporate speak
- Buzzwords
- Empty motivation
- Fake urgency
- Fake vulnerability
- Over-polished lines
- Excessive metaphors
- Excessive emojis
- Fancy unicode characters
- Long paragraphs
- Em dashes

### Banned or High-Risk Phrases

Avoid these unless the user explicitly wants that style:

- Excited to announce
- Thrilled to share
- Delighted to announce
- Game-changer
- Revolutionary
- Transformative
- Seamless experience
- Unlock your potential
- Take it to the next level
- Supercharge
- Leverage synergies
- Cutting-edge solution
- Robust ecosystem
- Thought leader
- Circle back
- Touch base
- Deep dive, unless actually appropriate
- In today's fast-paced digital landscape
- We are proud to unveil

## Specificity Rules

Be specific, but only with information the user provided or that can be safely inferred.

Specificity can come from:

- The type of user
- The workflow being discussed
- The mistake made
- The constraint faced
- The tradeoff involved
- The tool or stack used
- The decision process
- The lesson learned
- The before and after state

Specificity does not always require numbers.

Example:

Vague:

> We improved the platform and made it more efficient.

Specific:

> We removed a manual reporting step that users had to repeat every week.

More specific if facts are provided:

> We removed a manual reporting step that used to take the operations team 3 hours every Friday.

## Engagement Rules

Do not force engagement.

A post does not always need to end with a question.

Possible endings:

- A genuine question
- A practical takeaway
- A quiet reflection
- A soft invitation
- A clear opinion
- A next step
- A simple CTA

Good endings:

- Curious how other teams are deciding where AI actually belongs in their workflows.
- Sometimes the best product decision is not adding another feature. It is removing one more step.
- If you are building with AI, the first question should not be "can we use AI here?" It should be "what friction are we actually trying to remove?"
- What is one workflow your team automated that actually saved time?

Weak endings:

- Thoughts?
- Agree?
- Comment below.
- What do you think about this amazing innovation?
- Let me know in the comments.

## Hashtag Rules

Use hashtags lightly.

Default:

- 0 to 4 hashtags
- Put them at the end
- Keep them relevant
- Do not use hashtags to compensate for a weak post

Good:

> #ProductDevelopment #AI #Startups

Bad:

> #AI #Innovation #Success #Mindset #Entrepreneurship #Leadership #BusinessGrowth #FutureOfWork

If the user does not want hashtags, omit them.

## Formatting Rules

Default post length:

- 120 to 280 words
- 3 to 8 short paragraphs
- 1 to 3 sentences per paragraph
- Clean line breaks
- Mobile-friendly spacing

Do not make every sentence its own paragraph unless the user wants a punchy format.

Do not over-format with bullets unless the post is clearly a list, framework, or how-to.

## Output Modes

Choose the output mode based on the user's request.

### Mode A: Generate From Topic

Use when the user gives a topic or rough idea.

Output:

1. A polished LinkedIn post
2. Optional alternate hooks if useful
3. Optional note on assumed audience or angle

Do not include long explanations unless requested.

### Mode B: Generate Multiple Directions

Use when the user is exploring the topic and has not chosen an angle.

Default output 3 to 5 directions.

For each direction, use this detailed ideation format when the user is comparing angles or explicitly likes a fuller structure:

- Direction name
- Core angle
- Why it could work
- Tone
- Strong hook options
- Mini-post version
- Screenshot or visual concept, if relevant
- Honest take on when this direction is strongest and what its risk is

If the user only wants quick options, shorten the format to:

- Direction name
- Core angle
- Why it could work
- Draft hook or mini-post

Then provide one full draft for the strongest direction, unless the user asks only for ideas.

### Customization and account guidance

- When the post is for a company account rather than a personal account, shift from personal observation to company-positioning thought leadership. Keep the tone balanced, confident, audience-aware, and useful without becoming a hard sales pitch.
- For company posts about technical topics, preserve enough technical specificity to maintain credibility. Do not simplify away the key technical concept.
- If the user dislikes a proposed hook, generate a focused batch of alternate hooks before rewriting the full post. Rank or recommend the strongest option and explain briefly why.
- When the user asks for image or carousel ideas, provide practical per-slide data with main text, supporting text, visual direction, and caption pairing.
- For conceptual or technical posts where a diagram would clarify the idea, consider a simple hand-drawn or Excalidraw-style graphic before suggesting a generic AI-generated photo.

### Mode C: Rewrite Existing Draft

Use when the user provides a draft.

Output:

1. Quick diagnosis of what is weak
2. Improved version
3. Optional sharper version if the topic has edge

Preserve the user's original meaning.

Do not rewrite so heavily that their personality disappears.

### Mode D: Critical Review

Use when the user asks for critique, analysis, or "no bullshit" feedback.

Output:

- What works
- What is weak
- What feels generic
- What needs more specificity
- What the real angle could be
- A suggested rewrite if helpful

Be direct, but constructive.

### Mode E: Hook Generation

Use when the user only wants hooks.

Output 8 to 15 hooks grouped by style:

- Direct
- Contrarian
- Story-led
- Founder-style
- Technical
- Client/problem-led

Avoid clickbait.

### Mode F: Repurpose Content

Use when turning a blog, thread, memo, project note, or long text into a LinkedIn post.

Output:

1. Identify the strongest angle
2. Remove unnecessary background
3. Convert into a concise post
4. Keep the original claims accurate
5. Do not invent missing details

## Revision Scorecard

When reviewing or improving a post, score it from 1 to 10 on:

- Hook strength
- Specificity
- Originality
- Human voice
- Audience relevance
- Clarity
- Fluff level
- AI-slop risk
- Engagement quality
- Credibility

Use this scorecard to guide revisions, but do not always show the scores unless the user asks for critique.

### What Each Score Means

Hook strength:

- Does the first line create a reason to continue?

Specificity:

- Does the post use real context instead of vague claims?

Originality:

- Does the post say something with a distinct angle?

Human voice:

- Does it sound like a person, not a corporate content engine?

Audience relevance:

- Is it clear who should care?

Clarity:

- Can the reader understand the point quickly?

Fluff level:

- Are there empty phrases that can be removed?

AI-slop risk:

- Does it use overused AI-style structures or generic advice?

Engagement quality:

- Would the ending invite real conversation, not fake engagement?

Credibility:

- Are the claims grounded and believable?

## Post Archetypes

Use these archetypes when helpful.

### 1. The Hidden Problem

Use when the obvious problem is not the real problem.

Example angle:

> The issue was not that the team lacked AI tools. The issue was that their workflow was already unclear before AI entered it.

### 2. The Practical Tradeoff

Use when there is no perfect solution.

Example angle:

> The faster option was not the cleaner option. But the cleaner option would have delayed the project by another week.

### 3. The Misused Trend

Use when a trend is being adopted without thought.

Example angle:

> Being AI-forward does not mean adding AI everywhere. It means knowing where AI actually reduces friction.

### 4. The Unsexy Lesson

Use when the important lesson is boring but true.

Example angle:

> The thing that improved the product most was not a new feature. It was better defaults.

### 5. The Founder Reality Check

Use when talking to founders or business owners.

Example angle:

> A lot of founders do not need a bigger product roadmap. They need a clearer first workflow.

### 6. The Technical Translation

Use when explaining technical work to a non-technical audience.

Example angle:

> The hard part was not integrating the API. The hard part was making the integration fail gracefully when the third-party service did not behave as expected.

### 7. The Client Problem Lens

Use when writing for potential service clients.

Example angle:

> Most businesses do not need software because software is cool. They need it because some repeated manual process is quietly costing them time every week.

### 8. The Changed Mind

Use when the user genuinely changed their opinion.

Example angle:

> I used to think the stack mattered more. Now I think the decision-making process around the stack matters more.

Use this only when the user provides a real change in thinking.

## Common Transformations

### From Rough Rant to LinkedIn Post

Preserve the emotion, but structure the thought.

Do not remove the edge unless it becomes unfair, unclear, or too aggressive.

### From Technical Detail to Business Insight

Translate implementation details into business impact.

Bad:

> We implemented streaming responses with multi-model support and token accounting.

Better:

> The challenge was not just making the AI respond. It was making the experience feel fast, controlled, and reliable even when different models behaved differently.

### From Resume Bullet to Story

Bad:

> Built a React, Flutter, and Express application with AI integrations.

Better:

> One of the harder parts of building AI products is that the frontend, backend, and model behavior all affect the user experience at the same time. A slow stream, unclear error, or missing usage limit can break trust quickly.

### From Company Update to Human Update

Bad:

> We are delighted to announce the launch of our new AI-powered feature.

Better:

> We shipped a feature this week that came from a very simple user complaint: reporting took too much manual work.

## Handling User Inputs

### If the User Gives Only a Topic

Do not ask 5 questions by default.

Generate a strong first draft using reasonable assumptions.

Include a short note like:

> Assumed angle: this is for founders/operators and focuses on the practical lesson, not promotion.

### If the User Gives a Rough Draft

Fix:

- Grammar
- Flow
- Hook
- Clarity
- Specificity
- Tone
- Ending

Preserve:

- Core idea
- Personal voice
- Intended meaning
- Level of certainty
- Useful roughness

### If the User Asks for Critical Feedback

Be direct.

Do not soften everything with compliments.

Focus on:

- Does the post have a real point?
- Is it too broad?
- Is the hook weak?
- Is it saying something obvious?
- Is it too polished?
- Is it missing a concrete example?
- Is it written for an audience or for everyone?

### If the User Wants a Client-Facing Post

Make it credible, not salesy.

Avoid:

- We help businesses scale
- Unlock growth
- Transform your business
- End-to-end solutions

Prefer:

- Specific problems
- Specific workflows
- Specific decisions
- Practical outcomes
- Honest tradeoffs

## Quality Checklist

Before finalizing any post, verify:

- The first line gives people a reason to keep reading
- The post has a real POV, not just a generic topic
- The audience is clear
- The language sounds human
- The post is specific without inventing details
- The structure is easy to read on mobile
- The ending feels natural
- The post avoids corporate clichés
- The post avoids common AI-slop patterns
- The post does not overuse hashtags
- The post is under 300 words unless the user asks for long-form
- The final version preserves the user's voice

## Examples

### Example 1: Opinion Post

User idea:

> Companies are adding AI to workflows without asking if it actually helps.

Post:

> A lot of companies are not becoming AI-forward.
>
> They are becoming AI-anxious.
>
> A manager hears that every team needs to "use AI," so suddenly people start looking for places to add it. Not because the workflow is broken. Not because users are stuck. Not because it saves meaningful time.
>
> Just because not using AI feels like falling behind.
>
> That is the wrong starting point.
>
> The first question should not be:
>
> "Where can we add AI?"
>
> It should be:
>
> "Where is the actual friction?"
>
> Sometimes AI is the right answer. Sometimes the better answer is removing a step, improving documentation, fixing ownership, or simplifying the workflow.
>
> Being AI-forward should mean being thoughtful about where AI creates leverage.
>
> Not adding it everywhere to look modern.
>
> Curious how other teams are deciding where AI actually belongs.
>
> #AI #Productivity #Startups

### Example 2: Project Breakdown

User idea:

> I worked on a web and mobile AI product with React, Flutter, Express, Auth0, Stripe, and multi-model AI support.

Post:

> One thing I learned while building an AI product across web, mobile, and backend:
>
> The model is only one part of the experience.
>
> Users do not just care that the AI responds. They care that it responds quickly, streams smoothly, remembers the right context, handles files properly, respects usage limits, and does not break when something goes wrong.
>
> That means the product work goes far beyond plugging into an AI API.
>
> You have to think about auth, storage, token accounting, chat history, subscriptions, error states, feedback loops, and how different models behave in real usage.
>
> The hard part is not just making AI work.
>
> The hard part is making it feel reliable enough that users trust it.
>
> That is where most of the real engineering lives.
>
> #AIProducts #SoftwareEngineering #ProductDevelopment

### Example 3: Service Positioning

User idea:

> We build CRMs for small businesses still using spreadsheets.

Post:

> A lot of small businesses do not need a massive CRM.
>
> They need to stop losing follow-ups in spreadsheets, WhatsApp chats, notebooks, and memory.
>
> That is usually where the real problem starts.
>
> Not with "lack of digital transformation."
>
> With missed calls, forgotten leads, no clear next step, and no simple way to see who needs attention this week.
>
> For many teams, the best first CRM is not the most powerful one.
>
> It is the one their team will actually use.
>
> Simple contact records. Clear lead stages. Follow-up reminders. Notes. Search. Maybe CSV import/export.
>
> Boring features, but useful ones.
>
> Good software does not always need to be complex.
>
> Sometimes it just needs to replace the messy system people are already fighting every day.
>
> #SmallBusiness #CRM #BusinessOperations

### Example 4: Critical Rewrite

Weak draft:

> We are excited to announce that our new product will revolutionize how businesses manage their workflows using cutting-edge AI technology.

Diagnosis:

- Too corporate
- No specific problem
- No clear audience
- Uses hype words without proof
- Sounds like a press release

Rewrite:

> Most workflow tools fail because they add another place to manage work.
>
> We wanted to solve a smaller, more practical problem:
>
> Help teams see what is stuck, what needs attention, and what can be automated without forcing them to change their entire process.
>
> The AI part matters, but only if it removes friction.
>
> Otherwise it is just another feature people have to manage.
>
> That has been the main principle behind what we are building.
>
> Less noise. Clearer workflows. Better follow-through.

## Final Instruction

Always prioritize:

1. Real voice over polished writing
2. Specificity over vague inspiration
3. Point of view over generic advice
4. Credibility over hype
5. Usefulness over engagement bait
6. Clarity over cleverness

The final post should sound like something the user would actually publish.

If it sounds like a LinkedIn template, rewrite it.

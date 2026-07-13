---
name: email-polisher
description: Draft, polish, rewrite, and tone-shift email messages for workplace, academic, administrative, and relationship-sensitive contexts. Use when Codex needs to improve clarity, tact, professionalism, warmth, brevity, directness, or formality in an email; map a requested tone such as collegial, respectful, formal, diplomatic, warm, concise, or assertive to the wording; or provide several alternatives when the user does not specify a tone.
---

# Email Polisher

## Overview

Draft or revise emails so they sound intentional, context-aware, and easy to send. Preserve the user's facts, goal, and relationship cues while adapting tone, structure, and level of directness.

## Workflow

1. Identify the task:
   - Draft from bullets, notes, or a brief instruction.
   - Polish an existing email without changing the core message.
   - Rewrite in a different tone.
   - Shorten, soften, strengthen, or clarify a message.
2. Identify the context:
   - Who is the sender and who is the recipient?
   - What is the relationship: peer, manager, professor, client, recruiter, friend, or mixed audience?
   - What is the email trying to accomplish: request, update, follow-up, apology, scheduling, decline, reminder, thanks, escalation, or negotiation?
3. Check whether the user specified a tone explicitly. Accept:
   - A tone word such as `collegial`, `respectful`, or `formal`
   - A closely related instruction such as `make this warmer`, `more tactful`, `less stiff`, or `more concise`
   - A numeric tone code from [references/tones.md](references/tones.md)
4. If no tone is specified, provide multiple strong options instead of picking one silently.
5. Return send-ready email text. Keep details consistent with the source and do not invent facts, promises, attachments, timelines, or prior conversations.

## Output Rules

- Preserve the user's intent unless they explicitly ask to change it.
- Improve grammar, flow, and structure without flattening the message into generic corporate language.
- Keep sensitive emails tactful. Prefer calm precision over dramatic wording.
- Match salutation and sign-off to the requested tone and relationship.
- When polishing existing text, keep the original level of specificity unless clarity requires a small change.
- When the user asks for brevity, shorten aggressively while retaining the ask, decision, or next step.
- When the user supplies rough notes instead of a draft, infer a clean email structure: subject line if useful, greeting, purpose, key details, clear ask, and closing.

## Tone Handling

Read [references/tones.md](references/tones.md) whenever the user asks for a specific tone, gives a numeric code, or asks for multiple versions.

Apply these defaults:

- If the user names one tone, provide one polished version in that tone.
- If the user names two tones, either blend them naturally or provide two versions if the combination is awkward.
- If the user gives no tone, provide 3 versions:
  - `Collegial`
  - `Respectful`
  - `Formal`
- If the email is sensitive and the user gives no tone, bias the three versions toward tact and professionalism rather than playfulness.

## Response Format

Use a clean, copy-ready format.

For one version:

```text
Subject: ...

Hi/Hello ...,

...

Best,
...
```

For multiple versions, label each option clearly:

```text
Version 1 - Collegial
Subject: ...
...

Version 2 - Respectful
Subject: ...
...
```

After the drafts, add a one-line note only if it helps the user choose between versions. Do not add writing advice unless the user asks for explanation.

## Clarification Rule

Ask a brief follow-up only when a missing fact would materially change the email, such as:

- the recipient is unknown and the tone depends on status or familiarity
- the user wants a response to a message that is not included
- the email requires a concrete fact the user has not given

Otherwise, make the smallest reasonable assumption and proceed.

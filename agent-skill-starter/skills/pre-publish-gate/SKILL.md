---
name: pre-publish-gate
description: >-
  Mandatory check before any text goes outside: posts, captions, emails, product
  descriptions, landing pages. Not for chat answers to the owner or internal notes.
---
# Pre-publish gate

## When
Any text that people outside will read. Run it **before** asking for approval, so the approver sees the final version.

## Checks (all must pass)
1. **Facts:** Every number, price, date and claim has a source you opened in this task. Remove anything you cannot back up.
2. **No invented proof:** no made-up testimonials, client names, case studies or "used by 1,000 businesses".
3. **Concrete:** at least one real name, number, place or scene per paragraph. Abstract text reads like a machine wrote it.
4. **Openers and closers:** no "In today's fast-paced world", no "In conclusion". Start with the point, end with the next step.
5. **Filler words:** cut words like "seamless", "robust", "unlock", "leverage", "delve" unless they are literally true.
6. **Rhythm:** mix short and long sentences. Not every list has three items.
7. **Punctuation:** no em dashes as sentence glue, no chat-window bullets, no emoji headlines.
8. **Platform fit:** length, hashtags and links follow [PLATFORM_RULES] (e.g. max 5 hashtags, link only in bio).
9. **Privacy:** no addresses, phone numbers, emails or names of private people without consent.
10. **Read it aloud.** Would you say it to a customer like that? If not, rewrite.

## Output
Give [OWNER] the final text, a 1-line pass/fail per check, and the sources. If a checker script exists ([CHECK_COMMAND]), add its score and the threshold ([THRESHOLD]).

## Fill in
[OWNER], [PLATFORM_RULES], [CHECK_COMMAND] (optional), [THRESHOLD] (e.g. 85/100)

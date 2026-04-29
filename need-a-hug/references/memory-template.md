# Optional Comfort Memory Template

Use this only when the user explicitly asks to initialize or remember comfort context.

Do not infer these fields from local files, OS usernames, Git config, account metadata, or email addresses.

```markdown
# need-a-hug memory

preferred_name:

## User-stated preferences

- 

## Gentle context notes

- 

## Do not assume

- 
```

Recommended prompt. Use the matching-language version only. Do not output language labels.

For English:

```text
Sure.

What should I call you?

It is okay if you would rather not say. We can keep going.
```

For Chinese:

```text
可以。

以后我可以怎么称呼你？

不想说也没关系，我们直接继续。
```

Privacy rules:

- Store only what the user explicitly asks you to remember.
- Do not ask for country/region during initialization.
- Do not infer country/region from language, timezone, IP assumptions, file paths, account metadata, or cultural cues.
- Do not store medical history, diagnoses, trauma details, crisis details, or third-party private information.
- Do not store speculative labels such as "avoidant", "depressed", "procrastinator", or "anxious type".
- If the host product has a memory system, prefer that system.
- If local storage is appropriate, use `~/.need-a-hug/memory.md`.

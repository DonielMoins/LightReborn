# Light Reborn — Agent Instructions

This repository is a private journal of quotes and reflections, with one Markdown file per entry.

## Required entry format

- Follow `ENTRY_TEMPLATE.md`.
- Save entries in `entries/YYYY-MM-DD-short-title.md`, using a lowercase, hyphenated title in the filename.
- Include a title, `Date: YYYY-MM-DD`, `Author: ...`, and the entry body.
- Use ISO 8601 calendar dates (`YYYY-MM-DD`). Use the date supplied by the user; otherwise obtain the current local date from the system. Preserve existing dates unless the user requests a correction.
- Default to `Author: OROGLORIEUS` unless the user explicitly names another author. OROGLORIEUS is the author's known name; their real name is unknown. Never invent an identity or attribution.
- The entry body must contain 1–300 words, inclusive. Count whitespace-separated words in the body only, excluding the title, date, author, and Markdown formatting markers.
- Use correct grammar, spelling, punctuation, and consistent Markdown formatting. Use ordinary paragraphs for reflections and blockquotes for quotations.
- Preserve the meaning and voice. Do not silently rewrite a supplied quotation: propose any wording corrections for approval. If the body exceeds 300 words, ask the user to approve a shortened version; never truncate it silently.

## Entry workflow

1. Ask the user for the name of each new entry before creating its file, unless they have already explicitly supplied a name. Do not invent a title or infer approval from the quoted text. Existing entry titles do not need to be requested again.
2. Prepare the entry using the template, the correct date, and the default or explicitly supplied author.
3. Check the required fields, valid date, body word count, grammar, formatting, and filename. Never overwrite another entry; ask for a distinct title if the filename already exists.
4. Show the proposed entry and word count. Resolve any requested wording changes before committing.
5. Ask for explicit approval to auto-commit the current entry or batch. Default to leaving changes uncommitted; do not install automatic commit hooks or assume standing permission. Ask separately whether to push, or offer an explicit combined commit-and-push choice.
6. After approval, stage only the approved files and commit them. Push only if authorized. Verify the resulting commit and, if pushed, read back the remote commit and entry before reporting success.

Apply the same validation and commit-approval rules when editing existing entries. Do not change unrelated entries or add application code, dependencies, or automation for this journal.

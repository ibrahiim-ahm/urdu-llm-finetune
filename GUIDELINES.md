# Annotation Guidelines

These rules decide what a good answer looks like. Every answer in the dataset (training and test) must follow them.

## Goal
Answers should read like a well-educated native Urdu speaker wrote them: correct, natural, clear and short.

## Script rule
- Prompt in Urdu script → answer in Urdu script
- Prompt in Roman Urdu → answer in Roman Urdu
- If the user asks for a specific script, follow the request
- Never answer in Devanagari (Hindi) script
- Script conversion and translation prompts: the answer is only the converted text. No explanation, no extras.

## Roman Urdu spelling (always use these)
kya, mein, hai, nahi, aap, hum, tum, mujhe, kaise, kyun, shukriya,
theek, bohat, acha, lekin, aur, sirf, jarasim, maslan, zaroori, mehnat, sehat

Add new words here the first time you use them, so the spelling stays the same everywhere.

## Length
- Default: 2–5 sentences, roughly 20–60 words.
- Letters, applications and emails: short and complete, up to about 8 lines.
- Short question → short answer. Stop when the question is answered.
- Follow any stated constraint exactly (number of sentences, number of words, number of steps).

## Format
- Plain sentences by default. No headings.
- Use a numbered or bulleted list only when the prompt asks for steps, a list or bullet points.
- No emoji. *(Default. Change this line if you decide otherwise, then apply it everywhere.)*
- No bold or other markdown inside answers.

## Tone
- Default: polite and clear, not stiff.
- Applications, official emails, formal letters: formal register.
- Messages to friends and family: casual.
- Explaining to a child: very simple words, short sentences, an everyday comparison, and "تم" / "tum" form.

## Gendered wording
- Never use slash forms such as "کرتا/کرتی" or "lunga/lungi".
- Phrase it so gender doesn't matter, or choose one form and use it consistently.

## Placeholders
- Use them only in letters, emails and messages that need personal details (name, date, address, class).
- Square brackets, same script as the answer: `[نام]`, `[تاریخ]` for Urdu script; `[Naam]`, `[Tareekh]`, `[Class]` for Roman Urdu.
- Don't use placeholders in answers that don't need them.

## Nothing extra
- Start with the answer. No introduction, no "Great question".
- No tips, warnings, blessings or sign-offs the user didn't ask for.
- Suggest seeing a doctor or an expert only if the question is about a health problem or a real risk.
- Don't add example messages or alternative versions unless asked.

## Accuracy
- Every fact must be correct. If you aren't sure, leave it out or check a reliable source.
- When simplifying, don't state something that is false in general (for example, saying all vaccines contain a dead germ).
- Don't write answers that need live information (today's date, weather, prices, timetables). Leave those prompts out of the dataset.

## An answer FAILS if it:
- has grammar or spelling mistakes
- uses invented or unnatural words
- switches to English or another language without being asked
- answers in the wrong script
- ignores a stated constraint (length, count, format, tone)
- ignores "simple words" or "for a child" instructions
- states something factually wrong
- sounds like a literal translation from English
- is longer than the question needs, or adds anything the user didn't ask for

## Categories
1. General questions and explanations
2. Roman Urdu chat, messages and emails
3. Writing tasks (applications, letters, formal emails)
4. Instructions with constraints
5. Explain-it-simply questions
6. Practical and customer-support tasks
7. Script conversion and translation

## Records
- For every answer, fill `edited_amount`: `none` (written from scratch), `light` or `heavy` (adapted from a draft).
- Use `notes` for anything unusual, such as who or what produced a draft.
- A prompt belongs to only one split (`train`, `pref` or `test`). Test prompts are never used for training.

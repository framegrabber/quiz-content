# quiz-content

Quiz files for the [quiz app](https://github.com/framegrabber/quiz), served via GitHub Pages at `https://framegrabber.github.io/quiz-content/`.

| Quiz | Link |
|---|---|
| Englisch · Green Line 1 · Personal pronouns and be | [öffnen](https://framegrabber.github.io/quiz/#src=https%3A%2F%2Fframegrabber.github.io%2Fquiz-content%2Fenglisch%2Fgreen-line-1%2Fbe-forms.json) |
| Englisch · Green Line 1 · Negative forms of be | [öffnen](https://framegrabber.github.io/quiz/#src=https%3A%2F%2Fframegrabber.github.io%2Fquiz-content%2Fenglisch%2Fgreen-line-1%2Fbe-negative.json) |
| Englisch · Green Line 1 · Yes/No questions and short answers | [öffnen](https://framegrabber.github.io/quiz/#src=https%3A%2F%2Fframegrabber.github.io%2Fquiz-content%2Fenglisch%2Fgreen-line-1%2Fbe-questions.json) |
| Englisch · Green Line 1 · Possessive determiners | [öffnen](https://framegrabber.github.io/quiz/#src=https%3A%2F%2Fframegrabber.github.io%2Fquiz-content%2Fenglisch%2Fgreen-line-1%2Fpossessive-determiners.json) |
| Englisch · Green Line 1 · There is / there are | [öffnen](https://framegrabber.github.io/quiz/#src=https%3A%2F%2Fframegrabber.github.io%2Fquiz-content%2Fenglisch%2Fgreen-line-1%2Fthere-is-are.json) |

A quiz link is `https://framegrabber.github.io/quiz/#src=<URL-encoded link to a quiz file>`.

## Adding a quiz

1. Write the file following [`docs/quiz-format.md`](https://github.com/framegrabber/quiz/blob/main/docs/quiz-format.md) in the app repo. Path: `<subject>/<book-or-topic>/<quiz>.json`.
2. Validate locally from the app repo: `npm run validate -- ../quiz-content`.
3. Push. CI validates every file; invalid files block publishing.

Write your own sentences; do not copy texts or exercises from textbooks.

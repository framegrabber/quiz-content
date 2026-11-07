# quiz-content

Quiz files for the [quiz app](https://github.com/framegrabber/quiz), served via GitHub Pages at `https://framegrabber.github.io/quiz-content/`.

Every quiz appears automatically on the [app's start screen](https://framegrabber.github.io/quiz/) under "Quizze entdecken". CI generates the list as [`catalog.json`](https://framegrabber.github.io/quiz-content/catalog.json) on every push to `main`; it is not committed.

A direct quiz link is `https://framegrabber.github.io/quiz/#src=<URL-encoded link to a quiz file>`.

## Adding a quiz

1. Write the file following [`docs/quiz-format.md`](https://github.com/framegrabber/quiz/blob/main/docs/quiz-format.md) in the app repo. Path: `<subject>/<book-or-topic>/<quiz>.json`. The start screen groups quizzes by subject, grade, and `source`, and orders them by file path; prefix file names (`01-…`) to control the order.
2. Validate locally from the app repo: `npm run validate -- ../quiz-content`.
3. Push. CI validates every file and regenerates the catalog; invalid files block publishing. If a quiz uses a question type that was just added to the app, push only after the app's Pages deploy has finished; otherwise the live app rejects the quiz until it has.

Write your own sentences; do not copy texts or exercises from textbooks.

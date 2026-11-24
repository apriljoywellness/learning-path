# Learning Path

One page that holds April's whole free-AI-course plan and turns into a portfolio as courses are finished.

- **Page source:** `index.html` (the plan is the `COURSES` list near the bottom)
- **Repo:** https://github.com/apriljoywellness/learning-path (create it before the first push, see below)
- **Live:** Cloudflare Pages, auto-deploys on every push (URL added once it's connected)
- Replaces `projects/active/free-ai-learning-plan/learning-plan.html` (the old dated plan)

## Marking a course done

Tell Claude: "I finished [course]. I built [thing]. It solves [problem]. I learned [one line]."
Claude sets `done: "YYYY-MM-DD"` and the three portfolio fields, then commits and pushes. The page moves the course to the portfolio and shows the next one at the top.

You can also do it yourself on github.com: open `index.html`, click the pencil, edit the course, then commit.

## Adding a course

Add a line to `COURSES` in the order you want to take it. `provider` must be one of the tracks (Anthropic, Google, Code.org) or add a new track to `TRACKS` and `CATALOG`.

## First-time setup (one time only)

1. On github.com, signed in as apriljoywellness: **New repository** → name `learning-path` → **Public** → don't add a README → Create.
2. Tell Claude "repo's made" and Claude pushes the files.
3. In Cloudflare: **Workers & Pages → Create → Pages → Connect to Git** → pick `learning-path` → no build command, output folder `/` → Save and Deploy.
4. Bookmark the `.pages.dev` link it gives you.

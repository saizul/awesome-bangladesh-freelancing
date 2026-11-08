# Contributing

Thanks for helping Bangladeshi freelancers! This list stays useful only if it stays accurate.

## What to add

- Resources you have personally used or are confident exist and are useful for freelancers in Bangladesh.
- Free or clearly priced resources. **No affiliate or referral links**, no link shorteners, no tracking parameters.
- Official sources for anything about tax, banking, or law.

## Rules

1. One resource per line: `- [Name](https://url) - Short, neutral description.`
2. Keep descriptions factual. No hype, no "best" or "guaranteed income" claims.
3. Place the entry in the right section, alphabetically where practical.
4. Verify your URL before opening a PR:
   ```bash
   curl -sIL -o /dev/null -w '%{http_code}' --max-time 15 <url>
   ```
   Expect a 2xx or 3xx code. A 403 from bot protection is acceptable only for well-known sites; mention it in the PR.
5. Do not add anything that encourages policy violations (fake accounts, account renting, fake reviews). Such PRs will be closed.
6. Tax/legal entries: link official government or central-bank pages only, and do not summarise rules as advice.

## Automated link check

Pull requests that touch Markdown files, and a weekly scheduled run (Mondays, 03:00 UTC), run [lychee](https://github.com/lycheeverse/lychee) with the settings in [`lychee.toml`](lychee.toml). Responses such as 403, 429 and 999 are accepted because bot-protected sites often block automated checkers. A scheduled run that finds dead links opens an issue labelled `link-check`. To check locally: `lychee --config lychee.toml README.md`.

## Pull request checklist

- [ ] URL returns 2xx/3xx (or a justified 403)
- [ ] No affiliate/tracking parameters
- [ ] Neutral description, one line
- [ ] Not a duplicate

## Reporting dead links

Open an issue with the link and the section it is in, or send a PR removing it.

By contributing you agree your contribution is released under CC0 1.0.

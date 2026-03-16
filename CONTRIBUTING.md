# Contributing to Dark Night Rises CTF

Thanks for your interest in contributing! Here's how to get involved.

## Ways to Contribute

- 🐛 **Bug reports** — something broken? Open an issue
- 💡 **New challenge ideas** — suggest a vulnerability class
- 🎨 **UI improvements** — better visuals, animations, accessibility
- 📚 **Documentation** — clearer hints, better explanations
- 🌐 **Translations** — port the platform to other languages

## Adding a New Challenge

1. Copy an existing challenge file (e.g. `challenges/level5.html`) as a template
2. Keep the same structure: nav → breadcrumb → challenge-header → panels → flag-submit → success-overlay
3. Add your challenge to `challenges.html` in the grid
4. Link it from `index.html` challenge preview cards
5. Follow the flag format: `FLAG{your_flag_here}`
6. Submit a pull request with a description of the vulnerability being taught

## Code Style

- Pure HTML/CSS/JS — no frameworks, no build tools
- CSS variables for all colours (defined in `:root`)
- Share Tech Mono for code/terminal elements, Orbitron for headings
- Dark theme only — background `#030508`, accent `#00ffe7`

## Ground Rules

- All challenges must be **purely educational** and simulate vulnerabilities in-browser only
- No real exploits against live systems
- Keep it beginner-friendly — every challenge should have a hint path

## Reporting Issues

Open a GitHub Issue with:
- Which challenge/page is affected
- What browser and OS you're using
- Steps to reproduce the problem

# Webflyx

Webflyx is a fictional media streaming platform (a parody of Netflix) used as a hands-on project throughout the "Learn Git" course on [Boot.dev](https://www.boot.dev). 

I used this repository as a sandbox to practice real-world command-line Git and GitHub workflows using the Linux terminal (WSL/Ubuntu).

---------

### Areas Covered

* **GitHub CLI & Remote Management:** Authenticated using `gh auth login`, configured HTTPS/SSH protocols, and fixed remote tracking issues (`git remote add/set-url`).
* **Branching & Merging:** Created feature branches (`git checkout -b`), executed branch merges, resolved commit history, and edited commit messages inside the Nano terminal editor.
* **Pull Requests:** Pushed feature branches to GitHub, opened PRs, and merged changes back into `main`.
* **Git Configuration:** Configured local and global Git settings directly via CLI (such as setting `pull.rebase false` to control default pull behaviors).
* **Ignoring Secrets & Artifacts:** Built a `.gitignore` to prevent tracking secret credentials (`secure/`) and build outputs (`advert.html`).
* **Build Tooling:** Used `pandoc` in the command line to convert Markdown source files into HTML outputs to test tracking raw files while ignoring generated artifacts.

---------

### Project Files

* `classics.csv` — Acts as the mock database for Webflyx's movie catalog. Used to practice editing dataset files across different feature branches, merging updates, and resolving PRs.
* `advert.md` & `advert.html` — A marketing writeup for Webflyx ("Available on Floppy Disk!"). Used to practice converting source files into web-ready HTML using `pandoc`, while using `.gitignore` to keep the generated HTML file out of source control.
* `secure/` — Simulates a directory containing confidential company server credentials (`passwords.txt`), used to practice blocking sensitive data from being pushed to public GitHub repos.
* `.gitignore` — The configuration file instructing Git to ignore build artifacts (`advert.html`) and confidential directories (`secure/`).

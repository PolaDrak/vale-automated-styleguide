# Automated editorial linting architecture

This repository demonstrates a **Docs-as-Code** infrastructure designed to enforce editorial style guides automatically using **Vale**.

## Project architecture
Instead of reviewing documentation manually for style and grammar compliance, this project uses programmatic validation rules configured via YAML and Regular Expressions (Regex).

* `.vale.ini`: the central configuration file defining styles, scopes, and alert levels.
* `styles/Custom/`: directory containing custom-built corporate compliance rules.
* `document.md`: A sandbox file used to test and trigger linting errors in real-time.

## How to reproduce
1. Install Vale locally: `winget install errata-ai.Vale`
2. Clone this repository.
3. Open the folder in VS Code and run `vale document.md` in the terminal to view automated style violations.

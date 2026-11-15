# 🚀 024-mail-merge

A small Python script that turns one letter template and a list of names into one personalised letter per name. It is the mail merge project from day 24 of the Udemy *100 Days of Code* course.

## 📚 Table of Contents

- [Overview](#-overview)
- [Requirements](#-requirements)
- [Setup](#-setup)
- [Run](#-run)
- [Tests](#-tests)
- [License](#-license)
- [Links](#-links)
- [Appendix: Project documents](#-appendix-project-documents)

## 🧭 Overview

The script reads the guest names from a file, replaces the `[name]` placeholder in a letter template with each name, and writes one letter per guest.

| Path | Purpose |
| --- | --- |
| `main.py` | The mail merge script |
| `Input/Names/invited_names.txt` | The guest names, one per line |
| `Input/Letters/starting_letter.txt` | The letter template containing `[name]` |
| `Output/ReadyToSend/` | The generated letters, `letter_for_<name>.txt` |
| `docs/` | Project documents |
| `framework/` | The SQA and QC framework this project uses (submodule) |

It uses three string and file methods: `readlines()` to read the names, `strip()` to remove the trailing newline from each name, and `replace()` to substitute the placeholder.

## 📋 Requirements

- Python 3, to run `main.py`. No third-party packages are needed.

## 🛠️ Setup

Clone the repository with its framework submodule:

```bash
git clone --recurse-submodules ssh://git.tirsystem.com:10022/Tirsvad-Udemy-100-days-of-code/024-mail-merge.git
```

## ▶️ Run

From the project root:

```bash
python main.py
```

The generated letters appear in `Output/ReadyToSend/`. To change the guests or the letter, edit the files under `Input/` and run the script again.

## 🧪 Tests

The project has no automated tests. Check that the script compiles:

```bash
python -m py_compile main.py
```

## 📄 License

This project is licensed under the GNU Affero General Public License v3.0 (AGPL-3.0). See [LICENSE][license].

## 🔗 Links

- [Repository][repository]
- [Documentation][documentation]
- [Issue tracker][issues]

## 📎 Appendix: Project documents

The documents a newcomer needs, in reading order.

| Document | What it tells you |
| --- | --- |
| [Business Case][BC-001] | Why the project exists, its scope and success criteria |
| [Stakeholder Analysis][SA-001] | Who is involved; the stakeholder IDs used for owners and reviewers |
| [Project Plan][PP-001] | The gateways and their schedule |
| [Milestones][milestones] | One document per gateway: Go/No-Go criteria and tasks |
| [Artifact registry][registry] | Where each artifact type lives, the next version, the PO language and domain |
| [Traceability matrix][TM-001] | How the artifacts link and when each was last reviewed |

---

[repository]: https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/024-mail-merge
[documentation]: https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/024-mail-merge/wiki
[issues]: https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/024-mail-merge/issues
[license]: ./LICENSE
[BC-001]: ./docs/business-case.md
[SA-001]: ./docs/stakeholder-analysis.md
[PP-001]: ./docs/project-plan.md
[milestones]: ./docs/milestones/
[registry]: ./docs/artifact-registry.md
[TM-001]: ./docs/sqa/traceability-matrix.md

<div align="center">

# CSE120 Repository Template

Base template students will use to create their individual Lab / Project repositories.

</div>

## 🧭 Course / Section Metadata

Fill these in after creating your repo.

| Field | Value |
|-------|-------|
| Course | CSE120 Operating Systems |
| Term | <!-- e.g., Fall 2025 --> |
| Instructor | <!-- Name --> |
| Section / Time | <!-- e.g., Section 01, Tu/Th 10:30 --> |
| Student Name | <!-- Your full name --> |
| Student Email | <!-- UC Merced email --> |
| Student ID | <!-- 9-digit ID --> |
| Partner (if allowed) | <!-- Name / email or N/A --> |

## 📂 Repository Structure (Expected)

```
├── labs/
│   ├── lab01/
│   ├── lab02/
│   └── ...
├── projects/
│   └── phase01/
├── docs/
│   ├── design/        # design documents / architecture diagrams
│   ├── research/      # notes, citations, references
│   └── reports/       # final writeups
├── scripts/           # build, run, automation helpers
├── tests/             # test cases
├── .github/           # issue / PR templates, workflows
└── README.md
```

You may add additional folders when justified (update this README accordingly).

## ✅ Getting Started

1. Click "Use this template" on GitHub to create your private repository.
2. Clone your repo locally.
3. Fill in the metadata table above.
4. Create an initial branch (e.g., `setup`), never commit directly to `main` (unless instructed).
5. Open an Issue for each lab / feature before starting work.
6. Use Pull Requests to merge changes (each PR should reference at least one Issue).

## 🛠 Development Environment

| Tool | Recommended Version | Notes |
|------|---------------------|-------|
| Compiler / Toolchain | <!-- e.g., gcc 13.x --> | |
| Language Runtime | <!-- e.g., Python 3.12 --> | |
| Editor | VS Code | Install recommended extensions |
| OS Tested | <!-- Linux / macOS / WSL --> | |

Add environment setup instructions here:

```
git clone <your-repo-url>
cd <repo>
# any setup commands
```

## 🧪 Testing

Describe how to run your tests.

```
# example
make test
```

Include: what constitutes passing (e.g., all tests green, coverage threshold).

## 📜 Coding & Collaboration Conventions

Semantic commit messages (see `CONTRIBUTING.md` for full details):

```
<type>(optional scope): <imperative summary>

feat: add round-robin scheduler
fix(memory): correct null pointer dereference
docs: update lab02 instructions
test(scheduler): add starvation regression test
refactor: split pcb allocation logic
chore: update build script
```

Common types: feat, fix, docs, style, refactor, test, chore, perf, build, ci.

Branch naming pattern:
```
<type>/<short-kebab-feature>
e.g., feat/scheduler-phase1
```

Pull Request requirements:
* Linked Issue (e.g., Closes #12)
* Clear description of approach
* Testing evidence (logs / screenshots / results)
* Updated docs when behavior changes

## 🧾 Progress Tracking

Use GitHub Issues for tasks, bugs, enhancements. Use labels:
* `lab` – lab-specific work
* `bug` – defects
* `feat` – new functionality
* `research` – investigation / design tasks
* `discussion` – conceptual or design debate
* `urgent` – high priority

## 🗂 Documentation Expectations

Each lab folder should contain:
* `README.md` with objective, approach summary, build/run instructions
* Source code
* Test artifacts (inputs/outputs)

Design docs go in `docs/design/` as Markdown. Diagrams should be versioned (PlantUML, Mermaid, or exported images with source).

## 🧮 Grading Notes (Fill When Provided)

| Criterion | Weight | Notes |
|-----------|--------|-------|
| Correctness |  |  |
| Style / Readability |  |  |
| Documentation |  |  |
| Testing |  |  |
| Performance (if applicable) |  |  |

## 🔐 Academic Integrity

All work must follow UC Merced academic integrity policies. Do not copy solutions. Cite any external resources consulted.

## 🧩 FAQ (Add as Discovered)

| Question | Answer |
|----------|--------|
|  |  |

## 📌 Changelog (Optional)

Maintain a brief summary of major milestones.

| Date | Change |
|------|--------|
| YYYY-MM-DD | Initialized repository template |

---

Happy hacking! Keep this README current; graders will review it first.

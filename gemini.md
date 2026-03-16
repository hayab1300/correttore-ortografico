# Gemini DOE Framework

This project follows the DOE (Directive, Orchestration, Execution) architecture.

- `/directives` — SOP files. Consult before acting.
- `/execution`  — Python scripts. One script = one operation.
- `/temp`       — Intermediate data between scripts.
- `.env`        — Secrets. Never share or commit.

Rules:
1. Always read or create a directive before executing any task.
2. If a task requires more than 3 logical steps, write a Python script in /execution.
3. On errors, run the 4-step self-learning cycle and update the relevant directive.

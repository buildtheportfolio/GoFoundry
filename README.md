# Go Foundry

A hub for focused, self-contained Go projects covering backend engineering, concurrency, networking, APIs, CLI tools, and systems programming.

## Structure

```text
GoFoundry/
├── index.html
├── style.css
├── script.js
├── Ideas.md
└── projects/
    ├── _template/
    │   ├── go.mod
    │   ├── main.go
    │   └── README.md
    └── ...
```

The hub discovers project folders under `projects/` automatically. A folder is listed when it contains `go.mod`; `_template` is always excluded.

## Add a project

1. Copy `projects/_template/` to a URL-safe folder.
2. Update the module path in `go.mod`.
3. Build a focused idea from `Ideas.md`.
4. Run `go run .` and `go test ./...`.
5. Push the folder. No registry update is needed.

## Project rules

- One project per directory, independently runnable and testable.
- Use Go modules and the current stable Go release.
- Prefer the standard library and keep dependencies minimal.
- Keep project assets and documentation local to each project.
- Keep source code free of unnecessary comments.
- Deployment is manual. No GitHub Actions are required.

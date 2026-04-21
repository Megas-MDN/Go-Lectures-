# CLAUDE.md

Instructions for Claude Code working in this repository.

## About the project

Study repository for the **Go** language — examples, exercises, and lecture notes. Each directory/file tends to be self-contained (educational focus, not production).

## Stack

- Language: **Go** (1.26+)
- Tooling: `go`, `go test`, `go vet`, `gofmt`
- No default web framework — varies per example

## Conventions

- Idiomatic Go: follow `gofmt` and `go vet`.
- English for code identifiers; educational comments/notes may be in Portuguese.
- Prefer minimal, self-explanatory examples (this is a learning repo).
- Group each topic/lecture in its own directory when it makes sense (e.g. `01-basics/`, `02-goroutines/`).
- One `go.mod` per directory only when required; otherwise a single module at the root.

## Useful commands

```bash
go run ./path          # run an example
go test ./...          # run all tests
go vet ./...            # static analysis
gofmt -w .              # format everything
go mod tidy             # tidy dependencies
```

## Assistant guidelines

- **Do not create documentation files** (`README.md`, notes, plans) without an explicit request.
- **Prefer editing** existing files over creating new ones.
- Avoid unnecessary abstractions or defensive error handling — the focus is educational.
- Only add comments when the "why" is non-obvious.
- Before destructive actions (delete, reset, force-push), ask for confirmation.
- Commits follow **Conventional Commits** (`feat:`, `fix:`, `docs:`, etc.) and are only created when explicitly requested.

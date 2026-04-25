# Workspace instructions for AI coding agents

## Mandatory development checklist
- Lint: follow existing Blazor and CSS conventions in `.github/instructions/`; use any workspace formatter or analyzer if configured.
- Build: `cd SocOps && dotnet build`
- Test: no dedicated test project exists in this repo; validate behavior via `dotnet run` and code inspection.

## Project overview

This repo is a Blazor WebAssembly social bingo app on `.NET 10`.

- Source path: `SocOps/`
- Project file: `SocOps/SocOps.csproj`
- Startup: `SocOps/Program.cs`
- Run command: `cd SocOps && dotnet run`

## Core areas

- Pages: `SocOps/Pages/`
- Components: `SocOps/Components/`
- Services: `SocOps/Services/`
- Models: `SocOps/Models/`

## Key behavior

- `StartScreen.razor` begins the game flow.
- `GameScreen.razor` composes the board and tracks selection.
- `BingoLogicService` handles board generation and bingo detection.

## Existing workspace customizations

- `.github/instructions/css-utilities.instructions.md`
- `.github/instructions/frontend-design.instructions.md`
- `.github/agents/quiz-master.agent.md`
- `.github/prompts/setup.prompt.md`

## Guidance for agents

- Prefer links to `README.md`, `workshop/`, and existing `.github` instructions.
- Keep Blazor component structure intact and avoid unnecessary large rewrites.
- Validate changes with `dotnet build` and manual runtime checks when needed.

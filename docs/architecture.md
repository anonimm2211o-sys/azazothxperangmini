# UI Architecture

## Components

- `ScreenGui`: root container.
- `MainFrame`: compact panel.
- `Header`: title and drag area.
- `AutoCollectToggle` / `AutoSellToggle`: visual state controls only.
- `ActivityLogFrame`: recent UI messages.
- `MinimizedButton`: restores the panel after minimizing.

## Separation of concerns

Keep UI state and rendering separate from any game-specific logic. For a game you own or are authorized to modify, connect controls only to documented, permissioned systems and validate important actions on the server.

The current prototype intentionally contains no automation backend.

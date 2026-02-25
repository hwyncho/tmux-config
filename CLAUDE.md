# Claude Code Rules

> This document defines the rules that Claude Code must follow when working in this repository.

---

## Project Overview

Personal tmux configuration repository.

## File Structure

- `tmux.conf` — Main tmux configuration file

## Conventions

- `tmux.conf` is organized into sections separated by `# === ... ===` comment blocks:
  - **General** — Core tmux behavior settings
  - **UI** — Visual and display settings
  - **Keybindings** — Key binding definitions (including vi copy mode bindings)
  - **Statusline** — Status bar and pane border styling
- Each option should have a comment explaining its purpose
- Use `set-option` (not `set`) and `set-window-option` (not `setw`) for clarity
- Deprecated options should be commented out with a note

---

## Git Rules

- The Git rules for this repository are defined in `CONTRIBUTING.md` under "[Git Rules](./CONTRIBUTING.md#git-rules)" and act as the single source of truth. Branch naming, commit messages, and PR title/description must follow it.

- Branch names: `main`, `issue/{ISSUE}[-{SUMMARY}]`.
- Commit messages: `[<TYPE>] <Summary>`, then a blank line, then bullet details.
  - Types: `feat`, `enhance`, `refactor`, `docs`, `fix`, `style`, `chore`.
  - Summary: ≤ 50 characters, English, imperative, no trailing period.
  - Details: wrap at 72 chars, written in Korean or English.
  - Example:

    ```
    [feat] Add user authentication system

    - GitHub OAuth 2.0 PKCE 플로우 구현
    - JWT 토큰 기반 인증 미들웨어 추가
    - 사용자 세션 관리 기능
    ```

- PR title: `#<ISSUE_NUMBER> [<TYPE>] <Summary>` and must be in English.
  - Example: `#123 [feat] Add user authentication system`
- PR description: use the template provided in `CONTRIBUTING.md` and fill in the required sections.
- If any discrepancy arises, `CONTRIBUTING.md` takes precedence.

**Reference**: For more details, see [`CONTRIBUTING.md`](./CONTRIBUTING.md).

---

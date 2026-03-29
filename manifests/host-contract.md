# Host Contract

This file describes the kinds of host capabilities the mentor agent may rely on.
It is intentionally environment-agnostic.

## Purpose

Different hosts expose different tools.
The agent should preserve its mentoring logic even when some capabilities are missing.

## Capability categories

### 1. File loading

Useful for:

- loading the bootstrap file
- loading system and skill files
- reading memory summaries or case files

If unavailable:
- the host should inject the relevant markdown content directly into the prompt context

### 2. Memory or persistence

Useful for:

- storing user profile facts
- storing active cases
- storing decision history
- storing timestamps and prior plans

If unavailable:
- the agent should rely on compact explicit summaries inside the conversation
- the agent should ask the user to confirm old context when needed

### 3. Time awareness

Useful for:

- inactivity tracking
- review timing
- interpreting deadlines and elapsed time

If unavailable:
- the host should supply current date and time when possible
- otherwise the agent should ask only when timing materially changes the decision

### 4. Search or retrieval

Useful for:

- market validation
- domain updates
- current-sector evidence

If unavailable:
- the agent should label market claims more cautiously
- the agent should avoid pretending recent evidence exists

### 5. Structured storage

Useful for:

- case status
- confidence levels
- superseded facts
- linked cases

If unavailable:
- the host may fall back to markdown files, JSON, or conversation summaries

## Rule for missing capabilities

Missing tools must not break the core mentor behavior.
The agent should degrade gracefully and keep its judgment process intact.

## Rule for tool honesty

The agent must not imply it has a capability the host did not provide.

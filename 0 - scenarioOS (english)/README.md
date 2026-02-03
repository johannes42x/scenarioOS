scenarioOS – Usage & Workflow Guide

This document describes the practical workflow for using scenarioOS.
It is intended to live inside the scenarioOS folder and assumes no prior knowledge of MetaMemoryWorks.

---

## What scenarioOS does

scenarioOS allows you to export the *working state* of a long or complex conversation into a portable file, and later resume work from that state in a new session or even a different language model.

It does **not** preserve full chat history.
It preserves what matters for continuation.

---

## Typical use case

You are working in a long session:

- ideas accumulate
- assumptions are established
- constraints and decisions emerge
- tone and working style stabilize

Over time, the session becomes slow, noisy, or fragile.
You do not want to restart, because too much implicit state would be lost.

This is the moment scenarioOS is designed for.

---

## Basic workflow

### 1. Work normally

Start a conversation and work as usual.
There is no need to “prepare” for scenarioOS.

scenarioOS does not require special prompting during the session.

---

### 2. Trigger scenario export

When you want to preserve the current working state, do one of the following:

- Upload the scenarioOS engine file
- Ask the model to create a scenario from the current session

Typical phrasing examples:
- “Export the current scenario.”
- “Create a scenarioOS state for continuation.”
- “Preserve the working state as a scenario.”

The model will analyze the session and generate a **scenario file**.

---

### 3. Save the scenario file

The scenario file is the portable representation of your working state.

- Download it
- Keep it as-is (human-readable)
- Do not edit unless you know what you are doing

This file is the *only thing* scenarioOS needs for continuation.

---

### 4. Start a new session

Open a fresh session in the same or a different LLM.

Upload the scenario file.

Use a minimal instruction such as:
- “Continue from this scenario.”
- “Resume work using this scenario.”
- “Orient yourself using the scenario and proceed.”

You do **not** need to restate goals, tone, or constraints.

---

### 5. Continue working

The model should:

- pick up assumptions and decisions
- respect constraints
- maintain working style
- continue the task coherently

This is continuation, not replay.

---

## Cross-model usage

scenarioOS is model-agnostic.

A scenario file created in one model can be used in another, as long as file context is supported.

Exact phrasing may differ slightly, but the working state should transfer.

---

## When to create a new scenario

Create a new scenario when:

- the session becomes slow or unstable
- the task enters a new phase
- you want a clean checkpoint
- you want to switch models or environments

scenarioOS is not meant to run continuously.
It is meant to mark **transitions**.

---

## What scenarioOS does not do

scenarioOS does not:

- store memory automatically
- track users across sessions
- personalize models
- manage agents or tools
- replace judgment or decision-making

It is a continuity mechanism, not an automation system.

---

## Best practices

- Treat scenario files as checkpoints
- Keep older scenarios instead of overwriting
- Name scenario files meaningfully
- Use minimal prompts when resuming
- Let the scenario do the work

---

## In short

Work → Export scenario → New session → Continue.

That is the entire system.

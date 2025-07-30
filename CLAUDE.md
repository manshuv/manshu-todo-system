# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose
This is a personal todo management system using a simple markdown file (`todos.md`) to track tasks and their statuses.

## Todo Format and Status System
The todos.md file follows this structure:
- Each task is numbered and followed by a status
- Three possible statuses: "Done", "Doing", "To Do"
- If no status is specified, consider it "To Do"
- Tasks are organized in a numbered list format

## Common Operations
When managing todos:
- Always preserve the existing format and numbering
- Maintain the header section explaining the status system
- When adding new tasks, increment the numbering appropriately
- When updating status, only change the status text while preserving the task description
- Keep the "***Tasks start here***" delimiter intact

## File Structure
- `todos.md` - Main todo file containing all tasks and their statuses
- Tasks begin after line 13 (after the "***Tasks start here***" marker)

## Task Management Guidelines
- Read the current todos.md file before making any changes
- When marking tasks as "Done", preserve the original task text
- Sub-tasks (indented items) should maintain their relationship to parent tasks
- Always verify changes don't break the existing format or numbering system
- While adding a task - please add the date on which the task was added
- While closing the task please add the date on which the task was closed
- Also calculate how many days each task took and add that next to the completed date. 
-If you see tasks that have not been worked on for very long please ask me to update the status of those tasks and if I need any help with those
-Move all Done tasks to the Done section at the bottom. 

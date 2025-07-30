# Personal Todo Management System

A simple, markdown-based todo management system designed for use with Claude Code CLI.

## Overview

This system uses a single `todos.md` file to track tasks with a simple status-based approach. Tasks are organized in a numbered list format with clear status indicators and date tracking.

## Features

- **Simple Status System**: Three clear statuses - "Done", "Doing", "To Do"
- **Date Tracking**: Start dates and completion dates with duration calculation
- **Task Numbering**: Sequential numbering system for easy reference
- **Claude Code Integration**: Optimized for use with Claude Code CLI via `CLAUDE.md`

## File Structure

- `todos.md` - Main todo file containing all tasks and their statuses
- `CLAUDE.md` - Instructions for Claude Code on how to manage the todo system
- `README.md` - This documentation file

## Todo Format

Each task follows this structure:
```
[number]. [task description]. [status] (Started: [date])
```

### Status Options
1. **Done** - Task completed
2. **Doing** - Task currently in progress  
3. **To Do** - Task not yet started (default if no status specified)

### Example
```
1. Review quarterly metrics. To Do (Started: 2025-07-28)
2. Complete project documentation. Doing (Started: 2025-07-25)
3. Send team updates. Done (2025-07-30) - Duration: 2 days
```

## Task Management

### Adding Tasks
- New tasks are added with incremental numbering
- Start date is automatically added when task is created
- Default status is "To Do" if not specified

### Completing Tasks
- Tasks are moved to the "Done Tasks" section at the bottom
- Completion date and duration are calculated and added
- Task numbering in active list is adjusted

### Organization
- Active tasks remain in the main numbered list
- Completed tasks are moved to the "***Done Tasks***" section
- Tasks maintain their original description when completed

## Usage with Claude Code

This system is designed to work seamlessly with Claude Code CLI. The `CLAUDE.md` file provides specific instructions for:

- Preserving task format and numbering
- Managing task status transitions
- Calculating task duration
- Maintaining file structure

### Common Commands
- "Add task: [description]" - Adds new task with current date
- "Complete task [number]" - Marks task as done and moves to completed section
- "Show remaining tasks" - Lists all active tasks

## Best Practices

1. **Keep descriptions concise** - One line per task
2. **Use dates consistently** - All dates in YYYY-MM-DD format
3. **Maintain numbering** - Sequential numbering for easy reference
4. **Regular cleanup** - Periodically review old tasks for relevance

## Getting Started

1. Clone this repository
2. Start adding tasks to `todos.md`
3. Use Claude Code CLI for automated task management
4. Follow the format guidelines in `CLAUDE.md`

## File Templates

### New todos.md
```markdown
***This file contains [Your Name]'s ToDos***

***Each line is a task followed by status***

There are three statuses possible

1. Done
2. Doing
3. To Do

If an item does not have a status then consider it is To Do.

***Tasks start here***

1. Your first task. To Do (Started: YYYY-MM-DD)

***Done Tasks***
```

---

*This todo system was created for efficient task management with Claude Code integration.*
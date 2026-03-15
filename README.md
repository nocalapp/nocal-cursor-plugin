# Nocal Cursor Plugin

A [Cursor](https://cursor.com) plugin that connects your AI assistant to [Nocal](https://nocal.app), letting you search, create, and edit your notes without leaving the editor.

## Overview

Nocal is a second-brain app that combines notes and calendar. This plugin exposes Nocal's MCP server to Cursor's AI so you can:

- **Search notes** by keyword across your entire workspace
- **Browse recent notes** or filter by folder
- **Read a note** in full — including its plain-text content
- **Create new notes** in any folder
- **Edit notes** with conflict-safe patch operations

## Installation

1. Open Cursor and go to **Settings → Plugins → Browse Marketplace**
2. Search for **Nocal**
3. Click **Install**
4. When prompted, paste your **Nocal API token**
   - Find it in the Nocal app under **Settings → API Token**

## Usage

Once installed, just ask Cursor's AI to interact with your notes:

```
"Search my notes for the meeting recap from last Tuesday"
"Create a new note called 'Sprint planning' in my Work folder"
"What did I write about the API redesign?"
```

## MCP Tools

| Tool | Description |
|------|-------------|
| `notes_search` | Full-text search across your notes |
| `notes_list_recent` | List recently modified notes (optional folder filter) |
| `notes_get` | Get the full content and metadata of a note by ID |
| `notes_create` | Create a new note |
| `notes_patch` | Apply targeted edits to a note (with conflict handling) |

## Support

- **Nocal:** [nocal.app](https://nocal.app)
- **Issues:** [github.com/nocal-app/nocal-cursor-plugin/issues](https://github.com/nocal-app/nocal-cursor-plugin/issues)

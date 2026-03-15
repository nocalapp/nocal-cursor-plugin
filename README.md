# nocal Cursor Plugin

A [Cursor](https://cursor.com) plugin that connects your AI assistant to [nocal](https://nocal.app), letting you search, create, and edit your notes without leaving the editor.

## Overview

nocal is a second-brain app that combines notes and calendar. This plugin exposes nocal's MCP server to Cursor's AI so you can:

- **Search notes** by keyword across your entire workspace
- **Browse recent notes** or filter by folder
- **Read a note** in full — including its plain-text content
- **Create new notes** in any folder
- **Edit notes** with conflict-safe patch operations

## Installation

Add the following to your `~/.cursor/mcp.json` (global) or `.cursor/mcp.json` (project):

```json
{
  "mcpServers": {
    "nocal": {
      "url": "https://api.nocal.app/mcp",
      "headers": {
        "Authorization": "Bearer YOUR_NOCAL_TOKEN"
      }
    }
  }
}
```

Replace `YOUR_NOCAL_TOKEN` with your nocal API token, found in the nocal app under **Settings → API Token**.

## Usage

Once connected, ask Cursor's AI to interact with your notes:

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

- **nocal:** [nocal.app](https://nocal.app)
- **Issues:** [github.com/nocalapp/nocal-cursor-plugin/issues](https://github.com/nocalapp/nocal-cursor-plugin/issues)

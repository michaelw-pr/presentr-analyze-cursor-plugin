# Presentr Analyze for Cursor

Let Cursor's agent do media and document work for you: check, translate and re-time subtitles, transcribe audio and video, pull the text out of PDFs, scans and photos of handwriting (and translate it), read text aloud as an MP3, and dub audio or video into another language. Local files are uploaded by the agent; every paid job starts with a quote you confirm.

## What the plugin contains

- **An MCP server entry** (`mcp.json`) for Presentr Analyze's hosted server at `https://analyze.presentr.me/api/mcp`.
- **A skill, `analyze-media-and-documents`**, that tells the agent which tool fits the request, how to upload a local file, and to quote before any paid job.

Nothing runs on your machine: there are no hooks, scripts or packages.

## Sign in

The first time the agent uses Presentr Analyze, Cursor opens the browser to sign in with your Presentr Analyze account (Google or email). There is no API key to paste.

Without the plugin, the same server can be added by hand in `.cursor/mcp.json` or `~/.cursor/mcp.json`:

```json
{
  "mcpServers": {
    "presentr-analyze": {
      "url": "https://analyze.presentr.me/api/mcp"
    }
  }
}
```

## What you can ask

- "Check this SRT's timing." (free; finds overlaps, cues that are too fast or too long, and gaps)
- "Translate these subtitles into Spanish."
- "Re-time these subtitles to this audio."
- "Transcribe this recording."
- "Get the text out of this scanned PDF, and translate it into English."
- "Read this text aloud."
- "Dub this video into French."

## Cost

A free account includes 5 credits to try it. Before anything uses credits, the agent gets a quote (what the job will use and your balance) and asks you to confirm. A job never costs more than its quote, and work that isn't delivered isn't charged. Plans and credit packs: https://analyze.presentr.me/pricing

## Privacy

Presentr Analyze processes only the files, links and text the agent sends for a job; it doesn't see your conversation or the rest of your project. Jobs started by an agent expire 7 days after they were created, and their files are then scheduled for deletion. You can disconnect the app any time under Settings → Connected apps. Full policy: https://analyze.presentr.me/privacy

## Support

michael@presentr.me · https://analyze.presentr.me/developer/agents

Presentr Analyze is operated by T3 Interactive LLC.

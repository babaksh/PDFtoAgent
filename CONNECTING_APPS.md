# 🔌 Connect Hamilton MCP Server to Your Agentic Apps

Once your server is running (via **[Method 1: Portable Bundle](README.md#-method-1-standalone-portable-bundle-recommended-for-windows)** or **[Method 2: Docker Container](README.md#-method-2-docker-container-image-cross-platform)**), it exposes a standard **Streamable HTTP** FastMCP endpoint at:

```
http://127.0.0.1:8765/mcp  (or http://localhost:8765/mcp)
```

Below are step-by-step instructions and ready-to-paste configurations for all major AI clients.

---

## 1. Claude Desktop

Claude Desktop connects to HTTP MCP servers using the `mcp-remote` bridge.

### Locate Configuration File:
* **Windows (Standard):** `%APPDATA%\Claude\claude_desktop_config.json`
* **Windows (Microsoft Store):** `C:\Users\<YourUsername>\AppData\Local\Packages\Claude_pzs8sxrjxfjjc\LocalCache\Roaming\Claude\claude_desktop_config.json`
* **macOS:** `~/Library/Application Support/Claude/claude_desktop_config.json`
* *(Or directly inside Claude Desktop: `Settings ➔ Developer ➔ Edit Config`)*

### Configuration:
```json
{
  "mcpServers": {
    "Stock_Market_Barometer_Hamilton": {
      "command": "npx",
      "args": [
        "-y",
        "mcp-remote",
        "http://127.0.0.1:8765/mcp"
      ]
    }
  }
}
```
*(Requires Node.js for `npx`). Restart Claude Desktop and look for the hammer icon 🔨.*

---

## 2. ChatGPT Desktop (macOS & Windows)

### Option A: Via In-App Settings UI
1. Open ChatGPT Desktop.
2. Go to **Settings** (`Ctrl + ,` on Windows or `Cmd + ,` on macOS) ➔ **Apps & Connectors** (or **Plugins / Advanced**).
3. Click **Add MCP Server**.
4. Enter parameters:
   * **Name:** `Stock_Market_Barometer_Hamilton`
   * **Transport / Type:** `Streamable HTTP`
   * **URL:** `http://localhost:8765/mcp`
5. Click **Connect / Save**.

### Option B: Via Configuration File
```json
{
  "mcpServers": {
    "Stock_Market_Barometer_Hamilton": {
      "url": "http://localhost:8765/mcp",
      "transport": "streamable-http"
    }
  }
}
```

---

## 3. Google Antigravity

Antigravity natively supports Streamable HTTP MCP endpoints.

### Locate Configuration File:
* **Windows:** `%USERPROFILE%\.gemini\config\mcp_config.json`
* **macOS / Linux:** `~/.gemini/config/mcp_config.json`
* *(Or via UI: `Settings ➔ Antigravity ➔ MCP Servers ➔ Add Server`)*

### Configuration:
```json
{
  "mcpServers": {
    "Stock_Market_Barometer_Hamilton": {
      "serverUrl": "http://127.0.0.1:8765/mcp"
    }
  }
}
```

---

## 4. Cursor & Windsurf

### Option A: Via Cursor Settings UI
1. Open **Cursor Settings** (`Ctrl + Shift + J` on Windows/Linux or `Cmd + Shift + J` on macOS).
2. Go to **Features** ➔ **MCP Servers**.
3. Click **+ Add New MCP Server**.
4. Select **Type:** `SSE` / `HTTP` (Streamable HTTP).
5. Set **Name:** `Stock_Market_Barometer_Hamilton` and **URL:** `http://localhost:8765/mcp`.

### Option B: Via Global/Project Config (`.cursor/mcp.json`)
```json
{
  "mcpServers": {
    "Stock_Market_Barometer_Hamilton": {
      "url": "http://localhost:8765/mcp"
    }
  }
}
```

---

## 5. OpenClaw

Add the server block to your `openclaw.json` configuration:

### Locate Configuration File:
* **Windows:** `%USERPROFILE%\.openclaw\openclaw.json`
* **macOS / Linux:** `~/.openclaw/openclaw.json`

### Configuration:
```json
{
  "mcp": {
    "servers": {
      "Stock_Market_Barometer_Hamilton": {
        "url": "http://localhost:8765/mcp",
        "transport": "streamable-http"
      }
    }
  }
}
```

---

<div align="center">
  <a href="README.md">⬅️ Back to Main README</a>
</div>

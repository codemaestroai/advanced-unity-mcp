# Advanced Unity MCP from Code Maestro

**Control Unity with AI through natural language commands.**

Instead of clicking through menus and manually setting up GameObjects, just tell your AI assistant what you want and watch it happen automatically.

```
"Create a red material and apply it to a cube"
"Build the project for Android" 
"Make a new scene with a camera and directional light"
```

**Watch the video**

[![Watch the video](http://img.youtube.com/vi/EwBuDHmiHMA/0.jpg)](http://www.youtube.com/watch?v=EwBuDHmiHMA "Advanced MCP Integration for Unity - Powered by Code Maestro (Coming Soon)")

## Quick Start

**1. Install the Package**

Unity Package Manager → Add package from git URL for the version of Unity you are using

For **Unity 2020-2022**
```
https://github.com/codemaestroai/advanced-unity-mcp.git?path=Unity2020_2022
```

For **Unity 6+**
```
https://github.com/codemaestroai/advanced-unity-mcp.git?path=Unity6
```

**2. Connect Your AI**
- Go to `Code Maestro > MCP Dashboard` in Unity.
- **For Code Maestro Desktop App:** Select the "Code Maestro Desktop App" connection mode. The connection is automatic, and the dashboard will show the connection status.
- **For other clients (VS Code, Cursor, etc.):** Select the "Other Clients" connection mode, then click **Configure** next to your preferred client.
- Start giving commands!

**Supported MCP Clients:**
- **Code Maestro Desktop App** (uses Direct Connection)
- **GitHub Copilot (VS Code)**
- **Cursor**
- **Windsurf**
- **Claude Desktop**
- ...and any other MCP-capable copilot.

*Clients other than the Code Maestro Desktop App use the Relay Server connection, which is installed automatically.*

## What Unity MCP Can Do

**Core Editor Control** - Play/pause/stop game, execute menu items, read/clear console messages  
**Asset & Scene Management** - Create/modify/delete materials, prefabs, scripts, manage scenes and GameObjects  
**Build & Platform Tools** - Build settings, platform switching, Android Debug Bridge operations  
**Project Configuration** - Unity packages, project settings, PlayerPrefs, external tools  
**Performance Analysis** - Unity Profiler control for performance bottlenecks  

## Examples

- `"Check the console for any errors"`
- `"Create a script called PlayerMovement with WASD controls"`
- `"Switch the build target to iOS"`
- `"Add a rigidbody component to the selected object"`
- `"Create a new material with metallic properties"`
- `"Save the current GameObject as a prefab"`
- `"Clear all console messages and check for warnings"`

## How It Works

Unity MCP bridges your Unity Editor with AI assistants using the Model Context Protocol. It supports two connection modes, which can be selected in the MCP Dashboard:

- **Direct Connection (for Code Maestro Desktop App):** This is the recommended mode for Code Maestro users. The Unity Editor connects directly to the Code Maestro Desktop App's central hub. This method is faster and doesn't require a separate relay server.
  - **Unity MCP Connector:** Runs inside the Unity Editor to manage the connection.

- **Relay Server Connection (for other clients):** For clients like VS Code or Cursor, the bridge uses a local TCP server and a relay server.
  - **Bridge Server:** Runs in the Unity Editor and provides API access over a local TCP port.
  - **Relay Server:** A small background process that handles communication between the AI client and the Unity Bridge Server. It is installed automatically.

The setup is automatic. Simply choose your connection mode in the dashboard.

**💡 Tip:** When multiple Unity projects are open, your AI assistant will automatically connect to the most recently opened Unity Editor instance.

## Requirements

- Unity 2022+
- MCP Client (Such as GitHub Copilot or Cursor)

---

**Made by [Code Maestro](https://www.code-maestro.com) • [Join our Discord](https://discord.gg/bsFRAqATXz) • [Report Issues](https://github.com/codemaestroai/advanced-unity-mcp/issues) • [License](./LICENSE)**

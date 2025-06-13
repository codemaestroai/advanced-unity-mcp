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

Unity Package Manager → Add package from git URL:
```
https://github.com/codemaestroai/advanced-unity-mcp.git
```

**2. Connect Your AI**
- Go to `Code Maestro > MCP Dashboard` in Unity
- Click **Configure** next to your preferred MCP client
- Start giving commands!

**Supported MCP Clients:** Code Maestro, GitHub Copilot, Cursor, Windsurf, Claude Code

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

Unity MCP bridges your Unity Editor with AI assistants using the Model Context Protocol. Two components work together:

- **Bridge Server** - Runs in Unity Editor, provides API access
- **Relay Server** - Handles communication with MCP clients

The setup is automatic once you install the package and configure your MCP client.

## Requirements

- Unity 2022+
- MCP Client (Such as GitHub Copilot or Cursor)

---

**Made by [Code Maestro](https://www.code-maestro.com) • [Join our Discord](https://discord.gg/bsFRAqATXz) • [Report Issues](https://github.com/codemaestroai/advanced-unity-mcp/issues)**

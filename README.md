# @eldoraui/cli

Official CLI for Eldora UI components and MCP configuration.

<div align="center">
  <img src="https://github.com/eldorauiofficial/cli/blob/main/public/cli.png" alt="CLI" />
</div>

## Installation

### Global Installation

```bash
npm install -g @eldoraui/cli
```

### Using npx (Recommended)

```bash
npx @eldoraui/cli@latest install <client>
```

## Usage

### Install MCP Configuration

```bash
eldoraui install <client>
```

Or with npx:

```bash
npx @eldoraui/cli install <client>
```

### Supported Clients

- [x] cursor
- [x] windsurf
- [x] claude
- [x] cline
- [x] roo-cline

### Examples

```bash
# Install for Cursor
eldoraui install cursor

# Install for Claude Desktop
eldoraui install claude

# Install for Windsurf
eldoraui install windsurf
```

## Manual Installation

If you prefer to configure MCP manually, add this to your MCP config:

```json
{
  "mcpServers": {
    "@eldoraui/mcp": {
      "command": "npx",
      "args": ["-y", "@eldoraui/mcp@latest"]
    }
  }
}
```

## Development

```bash
# Clone the repository
git clone https://github.com/eldoraui/cli.git
cd cli

# Install dependencies
npm install

# Build the project
npm run build

# Run locally
npm start

# Development mode with auto-rebuild
npm run dev
```

## License

ISC

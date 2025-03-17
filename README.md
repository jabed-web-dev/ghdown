# ghdown (CLI Tool)

**A CLI tool to download GitHub repository files or folders**\
**Download a repository, folder, subfolder, or file from a GitHub repository URL or Path.**


## Install

```bash
npm install -g ghdown
deno install -g -RWN npm:ghdown
```

## Usage in CLI Command

```bash
ghdown -h|--help

Usage:
  ghdown <url> <path>?
  <url>   GitHub repository URL: <https://github.com/>?user/repo/<tree|blob>/branch/path/<folder|file>
          Use folder path: user/repo/<folder>                     Default branch: main
  <path>? Local directory path or filename: new-dir|new-filename  Default path: cwd+urlPath

          Download a repository, folder, subfolder or file from a GitHub repository URL or Path.
```

## Download commands
```bash
# Download folder with url
ghdown https://github.com/nodejs/node/tree/main/doc/api node-api
# with path
ghdown nodejs/node/tree/main/doc/api
ghdown nodejs/node/doc/api #(default branch main) work with folder path

# Download file with url
ghdown https://github.com/nodejs/node/blob/main/doc/api/index.md node-api.md
# with path
ghdown nodejs/node/blob/main/doc/api/index.md
```

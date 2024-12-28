# gitdown-cli (CLI Tool)

**Download a repository, folder, subfolders or file from a GitHub repository URL or Path.**


## Install

```bash
npm install -g gitdown-cli
```


## Usage in CLI Command

```bash
gitdown -h|--help

Usage:
  <url>   GitHub repository URL: <https://github.com/>?user/repo/<tree|blob>/branch/<folder|file>
          Use folder path: user/repo/<folder>   Default branch: main
          Download a repository, folder, subfolders or file from a GitHub repository URL or Path.
```

## Download
```bash
# download folder with url
gitdown https://github.com/nodejs/node/tree/main/doc/api
# with path
gitdown nodejs/node/tree/main/doc/api
gitdown nodejs/node/doc/api #(default main) work with folder path

# download file with url
gitdown https://github.com/nodejs/node/blob/main/doc/api/index.md
# with path
gitdown nodejs/node/blob/main/doc/api/index.md
```

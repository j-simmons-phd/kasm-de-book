# Installing VS Code

1. Add `- gantsign.visual-studio-code         # https://galaxy.ansible.com/gantsign/visual-studio-code` to `requirements.yaml`
1. Copy the contents of `vscode.yaml` into `playbook.yaml`, making sure to preserve order of the VS Code plays
1. Replace `- <insert list of extensions here>` with list of VS Code extensions to install (See [VS Code Extensions Marketplace](https://marketplace.visualstudio.com/vscode) to find extensions and their names)
1. Copy `../chrome/chrome.json` to the image root directory per https://stackoverflow.com/a/64460373
1. Add the following to the `docker-compose.yml` file

```
   # to get Chrome working per https://stackoverflow.com/a/64460373
    security_opt:
      - seccomp=./chrome.json
```
# start-a-blog

A template to get started with having your very own blog hosted for free by [Github Pages](https://pages.github.com/)

## Required steps

Note that my repository name is `start-a-blog`, yours may be different.

- update `blog/_config.yml` changing `root: /start-a-blog` to `root: /YOUR_REPOSITORY_NAME`
- generate your SSH key `ssh-keygen -t ed25519 -C githubdeploykeymyblog` so that `.github/workflows/gh-pages.yaml` can publish your work
  - Don't include a passphrase
- add the generated public key (.pub) to your repository configuration `Settings > Deploy Keys`
- add the generated private key to your repository configuration `Settings > Secrets` with the `Name` as `DEPLOY_KEY`

## Usage

This repository uses the [Hexo](https://hexo.io/docs/) tool to create a static site and github actions to automatically deploy to `https://YOUR_GITHUB_NAME.github.io/YOUR_REPOSITORY_NAME`. For my version, you can find the [deployment here](https://atable.github.io/start-a-blog/)

To begin writing, you should familiarise yourself with [Hexo's docs](https://hexo.io/docs/writing) now that the everything behind the scenes is operational. Simply push your changes and let the magic take care of the rest.

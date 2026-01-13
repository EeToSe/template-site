## Installing and Deploying

For installation and deployment details please refer to [INSTALL.md](INSTALL.md).

**TL;DR:**

1. [Use this template -> Create a new repository](https://github.com/new?template_name=al-folio&template_owner=alshedivat), naming it `<your-username>.github.io` (for user site) or any other name (for project site).

2. In this new repository, go to [Settings -> Actions -> General -> Workflow permissions -> **Read and write permissions**](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/enabling-features-for-your-repository/managing-github-actions-settings-for-a-repository#configuring-the-default-github_token-permissions)

3. Open `_config.yml` and set:

- `url: https://<your-username>.github.io`
- `baseurl: /project-name/`

Commit and push to `main`.

4. Wait for workflow to create/update `gh-pages`.

5.Let the Deploy workflow generate `gh-pages`, then go to [Settings → Pages]:

- Under **Build and deployment**
- **Source**: “Deploy from a branch”
- **Branch**: `gh-pages`
- **Folder**: `/ (root)`

6. visit: `https://<your-username>.github.io/project-name/`

# deploy-it-tools

Automated deployment of [IT Tools](https://github.com/CorentinTh/it-tools) to GitHub Pages.

## How it works

A GitHub Actions [workflow](.github/workflows/deploy.yml) runs **weekly** (every Monday at midnight UTC) and checks the upstream [CorentinTh/it-tools](https://github.com/CorentinTh/it-tools) repository for new releases. If a new version is found, it builds the project from source with the correct base path and deploys to GitHub Pages.

The workflow can also be triggered manually from the **Actions** tab with an optional **force** flag to redeploy even if the current version is up-to-date.

## Manual trigger

1. Go to **Actions** → **Deploy IT Tools**
2. Click **Run workflow**
3. Optionally check **Force deployment** to redeploy the current version

## Setup

1. In your repository settings, go to **Pages** → **Build and deployment** and set the source to **GitHub Actions**
2. Run the workflow manually for the first deployment

## License

This repository's configuration and workflow code is licensed under the [MIT License](LICENSE).

The deployed [IT Tools](https://github.com/CorentinTh/it-tools) application is licensed under [GPLv3](https://github.com/CorentinTh/it-tools/blob/main/LICENSE) by [Corentin Thomasset](https://github.com/CorentinTh).

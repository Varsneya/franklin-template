# Your Project's Title...
Your project's description...

## Environments
- Preview: https://main--{repo}--{owner}.hlx.page/
- Live: https://main--{repo}--{owner}.hlx.live/

## Installation

```sh
npm i
```

## Linting

```sh
npm run lint
```

## Local development

1. Create a new repository based on the `aem-guides-boilerplate` template and add a mountpoint in the `fstab.yaml`
1. The URL in fstab.yaml file will always follow the structure: https://dita-franklin-worker.adobeaem.workers.dev/{your_github_user_name}/{git_repository_name}/{branch_name}/{root_folder_name}
1. Add the [AEM Code Sync GitHub App](https://github.com/apps/aem-code-sync) to the repository
1. Create a Github App and give it all the repository permission(read and write or admin, whatever applicable highlest level permission is there), and install it on your repository.
1. Create Edge delivery service profile in AEM Guides.
1. Create Edge delivery service preset in AEM Guides and publish using the profile created in the previous step. This will add some sample data to your environment.
1. Install the [AEM CLI](https://github.com/adobe/aem-cli): `npm install -g @adobe/aem-cli`
1. Start AEM Proxy: `aem up` (opens your browser at `http://localhost:3000`)
1. Open the `{repo}` directory in your favorite IDE and start coding :)

## Important
1. If you change the working branch and root folder, the fstab.yaml file will also have to be updated with the correct branch_name and root_folder_name.
2. Making changes and committing to any .js, .css or any media file will push it to *.hlx.live site as well, be sure that you have tested your changes locally before committing them to your repo.

# Contributing

We welcome and appreciate all contributions from the community. Thank you for helping others grow and learn by sharing your media resources!

## Table of Contents

- [How Can I Contribute?](#how-can-i-contribute)
- [Setup - Git, GitHub](#setup---git-github)
- [Pull Request](#pull-request)
  - [Submitting a Pull Request](#submitting-a-pull-request)
  - [After Pull Request Merged](#after-pull-request-merged)
- [Keeping Fork Synced with Upstream](#keeping-fork-synced-with-upstream)
- [Resources](#resources)

## How Can I Contribute?

You can contribute by adding the media resource of your choosing under an existing category heading in repository [README.md](README.md). If a suitable category or subcategory does not exist, feel free to create one so others can follow.

## Setup - Git, GitHub

If you don't already have [Git](https://git-scm.com/) installed, install it first. You will need it to contribute.

### Installation

1. [Fork](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo) the repository.
2. Open a terminal, or "Git Bash" on Windows.
3. Use `cd` to move to the directory that you want to work in.
4. [Clone your repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository).
5. [Configuring the remote repository for your fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/configuring-a-remote-repository-for-a-fork).
6. Open the folder in your favorite editor. If you don't have one, try [Visual Studio Code](https://code.visualstudio.com/).

## Pull Request

Once you have finished making changes, you can submit a pull request to have your changes merged.

**🙋‍♂️ Please ensure your media resource supports the greater good of humanity, promotes sustainability, and/or encourages personal growth and positive perspectives.**

**📝 Remember to add your media resource to the Table of Contents section as well.**

### Submitting a Pull Request

Before you submit your Pull Request (PR) consider the following:

1. *Choose a category*: Add your resource under an existing category heading (h2, h3, or h4) in [README.md](README.md).

2. *Add new categories(**if needed**)*: If your media doesn’t fit an existing category or subcategory, feel free to create one so others can follow.

3. *Include a valid link*: Every resource must have a working link to an official source (publisher, platform, or creator).

4. *Ensure accuracy*: Only add valid, trustworthy resources. Double-check that links are active.

5. *Keep formatting consistent*: Use the following markdown formatting:

    ```markdown
    - **[Title of the Media](URL)** by *Author(s) or Creator(s)* – Short description.
    ```

6. Skip this step if you have completed [Setup - Git, GitHub](#setup---git-github). Otherwise, please complete it first and then return here.

7. In your forked repository, make your changes in a new git branch:

   ```bash
   git checkout -b add-book-atomic-habits main
   ```

   **Note**: We recommend your branch naming be the following format:

   ```bash
   add-<media-resource-type>-<media-resource-name>
   ```

8. Add/or edit your media resource.

9. Stage and commit your changes using a descriptive commit message.

   ```bash
   git add .
   git commit -m "Add book: Atomic Habits"
   ```

   **Note**: Keeping your commits to one media resource is recommended.

10. Push your branch to your remote fork:

   ```bash
   git push -u origin add-book-atomic-habits
   ```

11. In GitHub, send a pull request to `the-good-green-media-list:main`.

That's it! Thank you for your contribution!

### After Pull Request Merged

After your pull request is merged, you can safely delete your branch and pull the changes from the main (upstream) repository:

- Delete the remote branch on GitHub either through the GitHub web UI or your local terminal as follows:

  ```bash
  git push origin --delete add-book-atomic-habits
  ```

- Check out the main branch:

  ```bash
  git checkout main -f
  ```

- Delete the local branch:

  ```bash
  git branch -D add-book-atomic-habits
  ```

## Keeping Fork Synced with Upstream

- Update your local `main` with the latest changes from upstream:

  ```bash
  git pull --ff upstream main
  ```

- Fetch the latest changes from upstream:

  ```bash
  git fetch upstream
  ```

- Update your local `feature branch` with latest changes from upstream:

  ```bash
  git fetch upstream && git rebase upstream/main
  ```

## Resources

- [How to contribute to open source](https://opensource.guide/how-to-contribute/)
- [Contributing to a project](https://docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-project)
- [Using pull requests](https://help.github.com/articles/about-pull-requests/)
- [GitHub help](https://help.github.com)

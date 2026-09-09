# Public Repository Workflow

This repository documents the workflow used to create and publish it.

## 1. Install VS Code and extensions

1. Download and install [Visual Studio Code](https://code.visualstudio.com/).
2. Install useful extensions such as **Markdown All in One** and **Peacock** from the Extensions view.

## 2. Create a GitHub account and install GitHub Desktop

1. Sign up at [GitHub](https://github.com/).
2. Download and install [GitHub Desktop](https://desktop.github.com/).
3. Sign in to GitHub Desktop with your GitHub account.

## 3. Create the public repository and homepage

1. Create a new public repository on GitHub.
2. Add a top-level file named `index.html`.
3. Add a link whose visible text is `Link to repository` and whose target is the public repository URL:

```html
<a href="https://github.com/sandypandas/public-repo-2">Link to repository</a>
```

## 4. Stage, commit, and push changes

From the repository folder, run:

```bash
git add .
git commit -m "Describe the change"
git push origin main
```

GitHub Desktop can perform the same stage, commit, and push workflow through its interface.

## 5. Deploy with GitHub Pages

1. Open the repository's **Settings** on GitHub.
2. Select **Pages** in the **Code and automation** section.
3. Set the source to **Deploy from a branch**.
4. Select the `main` branch and the `/ (root)` folder, then save.
5. Open the published URL shown by GitHub Pages, usually:
	`https://sandypandas.github.io/public-repo-2/`

## 6. Collaborate through a pull request

1. Open **Settings > Collaborators** and invite a GitHub user.
2. The collaborator clones the repository, creates a branch, and makes a suggested change.
3. They push the branch and open a pull request against `main`.
4. Review the pull request, approve it, and select **Merge pull request**.
5. Delete the branch if it is no longer needed, then pull the merged changes locally.

## 7. Save and sync these instructions

Keep this `readme.md` at the repository top level. After editing it, run:

```bash
git add readme.md
git commit -m "Document repository workflow"
git push origin main
```

## Quarto extension

This repository also contains the `quarto-ext/fontawesome` extension under `_extensions/`. It was installed with:

```bash
quarto add quarto-ext/fontawesome
```

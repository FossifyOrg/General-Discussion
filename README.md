# Contributing to Fossify

Thank you for your interest in improving Fossify! 

To make the process as smooth as possible for everyone, please read the relevant section below.

## Reporting an issue or suggesting a feature

1.  This repository is for bugs and suggestions that affect **multiple** apps. For issues affecting only one app, use its separate repository.
2.  If you are reporting a bug, provide clear **steps to reproduce** it. Be sure to mention your app version, device model, and OS version.
3.  Ensure you're using the **latest app version** and have read the in-app FAQ before reporting.
4.  **Search first!** Check if the issue has already been reported by searching with relevant keywords.
5.  If a feature request already exists, add a "👍" to show your support. Avoid comments like `+1` or `I need this too!`, as they do not add useful information.
6.  If a bug is already reported and has the `needs reproduction` or `device/software specific` labels, feel free to add a comment with your device model and OS version.
7.  Please write all reports in **English**. Reports in other languages will be closed.

## Contributing code

1. **Issue first**

   - Before starting work, confirm there is an open issue for the task and that it is not tagged `needs triage`.
   - **Exceptions:** Critical, unclassified production-blocking bugs. Trivial changes, such as typos or broken links.

2. **Code style & formatting**

   - Always format code and optimize imports.
   - Follow existing naming and style conventions. Don't introduce a new style.
   - Prefix any new icon with `ic_`, use white vector drawables.
   - Always use braces, even for one-line `if`, `return`, or `continue` statements.

3. **Commit messages**

   - Use clear, descriptive commit messages.
   - Prefer [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/#specification).

4. **Theming & accessibility testing**

   - Test UI changes on all themes (Light, Dark, Black & White, System default on Android 12+) and with the largest system font size.

5. **CI and quality gates**

   - Ensure **all** CI checks pass (build, tests, lint, detekt, etc.) on your pull request.

6. **Completeness & readiness**

   - PRs must be well-researched, thoroughly tested, and production-ready.
   - No bare-bones or speculative PRs.

7. **Build configuration**

   - Changes to build configuration, dependencies, or target SDK versions require explicit prior approval.

> **Note:** Most pull requests will be **squash merged** unless they contain atomic changes worth preserving.

## Contributing translations

The best and preferred way to contribute translations is via Weblate.

- **Contribute on Weblate: [https://hosted.weblate.org/projects/fossify/](https://hosted.weblate.org/projects/fossify/)**

If you prefer to work directly on GitHub, you can follow the instructions below.

<details>
<summary><b>Click for GitHub translation instructions</b></summary>

### Editing an existing language file
1.  Log in to GitHub and navigate to the target language file (e.g., `app/src/main/res/values-es/strings.xml`).
2.  Click the pencil icon to edit the file.
3.  Modify only the text between `>` and `</string>`. Do **not** change the `name="..."` attribute or any comments.
4.  Escape any apostrophes with a backslash (`\'`).
5.  Add a clear commit message (e.g., "Update Spanish strings").
6.  Click **Propose file change**, then **Create pull request**.

### Adding a new language file
1.  Log in to GitHub and navigate to `app/src/main/res` in the app's repository.
2.  Click **Create new file**.
3.  In the path box, type the folder path `values-<language_code>/` (e.g., `values-de/` for German).
4.  Name the file `strings.xml`.
5.  Copy the entire contents of the default `app/src/main/res/values/strings.xml` into your new file.
6.  Translate the strings, making sure to escape apostrophes (`\'`).
7.  Add a clear commit message (e.g., "Add German translations").
8.  Press **Propose new file**, then **Create pull request**.

</details>

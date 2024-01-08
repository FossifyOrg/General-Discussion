# General-Discussion

A place for discussing all apps in general + anything else you want to say.

## FAQ

### How do I suggest an improvement, ask a question or report an issue?

1. This general discussion repository is used for bugs and suggestions that affect multiple apps. For issues affecting only 1 app, use its separate repository.
2. If you are reporting a bug, provide steps for reproducing, and mention your app and OS version.
3. Ensure you use the latest app version and read the in-app FAQ before reporting anything.
4. Check if the issue has already been reported. Use search with some keywords.
5. If the issue is already reported, give it an upvote to increase its priority.

---

## Contribution rules for developers

1. Every project contains a `.editorconfig` file, with definitions of required indentations, newlines, etc.
2. Always format the code (`Ctrl + Alt + L`) and optimize imports (`Ctrl + Alt + O`) before creating a pull request.
3. If you add a new icon, make sure it is prefixed with "ic_", it is white, and try using vectors.
4. If you change something in the UI, test the visibility with all themes, including Black & White and System default (Material You) on Android 12+. Test the changes by using the biggest system font size too.
5. Use the existing code style and naming conventions; do not bring your own style.
6. Always use brackets, even at 1 liner "if", "return" or "continue" statements, etc.
7. If you add a new model or work with Gson, test the build in release mode with Proguard enabled as well.
8. There is no real functionality change between build flavors, only some About button visibility differences, Rate Us dialog, and More Apps From Us buttons not showing up or so. The proprietary gallery build has a more advanced photo and video editor, while the FOSS one has a basic only.

If you try fixing a bug or adding a new feature, make sure that it is already reported at the given repository and the report is open and marked as a Bug or Feature Request. If the given issue is closed, chances are that we are not interested in the given feature, and your pull request will likely be rejected.

---

## How can I suggest an edit to a file?

Creating pull requests with some changes is a lot simpler than most people think. Most suggestions are related to translating strings, there are 2 ways to do it.

You can find our apps on Weblate at https://hosted.weblate.org/projects/fossify/, you can see untranslated strings there easily.

However, if you prefer the old-style file updating via Github, you can still do it. The process is the following:

1. Log in to GitHub.
2. Find the file with the strings (`app/src/main/res/values(-xx)/strings`, for example, the Italian translation of the Gallery is at https://github.com/FossifyOrg/Gallery/blob/master/app/src/main/res/values-it/strings.xml).
3. Click the pencil button at the top right corner of the file.
4. Edit the file with your suggestions.
5. Add a commit message under the file, to the text field which has a hint similar to "Update strings.xml". Just type in what you have done, for example, "updating Spanish strings".
6. Click `Propose file change`.
7. Click the green button `Create pull request`.
8. Thank yourself!

* Change only the string which is between ">" and `</string>`, _not_ the first one after the "name=" tag, also not the strings between `<!--` and `-->`.
* Please escape apostrophes, meaning you have to put a backslash before every apostrophe to make it look like: \\'

To find the proper language file at the Gallery, go to https://github.com/FossifyOrg/Gallery/blob/master/app/src/main/res, then look for a "values-[language code]" folder. Use the `strings.xml` file inside it. If you can't find your language code, the file might not be translated to your language at all yet, and you will have to create a whole new file.

---

## How do I add a new file?

You will most likely want to add a new file only if you translate an app into a new language. Doing it is actually not difficult at all, just read on.

1. Log in to GitHub.
2. Find the place where the new file belongs. If it's really a translation of the strings in a new language, go to `app/src/main/res`, for example https://github.com/FossifyOrg/Camera/tree/master/app/src/main/res.
3. At the top right corner click at `Create new file`.
4. After the `res` folder, you can type in your folder path. For creating a German translation just type in `values-de/` (where `de` is the country code). The new folder will be added automatically after typing the slash.
5. Add a file name, i.e., `strings.xml` (the path should look similar to the image below)
   <img src="https://github.com/FossifyOrg/General-Discussion/assets/36371707/a8aa4d5e-c0c1-4d10-b82b-8c7ec6d21e68" alt="Github new file path" width=75% />
7. Copy the contents of an already existing `strings.xml` file into the new file (for example, the content of https://github.com/FossifyOrg/Camera/blob/master/app/src/main/res/values/strings.xml).
8. Add your string translations.
9. Add a commit message under the file, to the text field which has a "Create new file" hint. Just type in what you have done, for example, "adding Spanish strings".
10. Press `Propose new file`.
11. Click the green button `Create pull request`.
12. Thank yourself!

* Change only the string which is between ">" and `</string>`, _not_ the first one after the "name=" tag.
* Please escape apostrophes, meaning you have to put a backslash before every apostrophe to make it look like: \\'


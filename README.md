# General-Discussion
A place for discussing all apps in general + anything else you want to say.

FAQ
---
## How do I suggest an improvement, ask a question or report an issue?
1. this General Discussion repository is used for bugs and suggestions that affect multiple apps. For issues affecting only 1 app use its separate repository
2. if you are reporting a bug, try giving steps for reproducing too. Also mention your app and OS version
3. make sure you use the latest app version and read the in-app FAQ before reporting anything
4. make sure the given thing isn't reported yet, you can also use Search with some keywords
5. if the thing you wanted to report has already been reported, don't forget giving it an upvote to increase its priority

<p>&nbsp;</p> 

## Contribution rules for developers
1. every project contains an .editorconfig file, it has definitions of required indentations, newlines etc
2. always format the code (Ctrl + Alt + L) and optimize imports (Ctrl + Alt + O) before creating a pull request
3. if you add a new string, add it into all languages. If you speak a language yourself, translate it. If not, just use the english version. Do not use machine translating
4. if you add a new icon, make sure it is prefixed with "ic_", it is white and try using vectors
5. if you change something in the UI, test the visibility with all themes, including Black & White and System default (Material You) on Android 12+. Test the changes by using the biggest system font size too.
6. use the existing code style and naming conventions, do not bring your own style
7. always use brackets, even at 1 liner "if", "return" or "continue" statements etc
8. if you add a new model or work with gson, test the build in release mode with proguard enabled aswell
9. there is no real functionality change between build flavors, only some About button visibility differences, Rate Us dialog and More Apps From Us buttons not showing up or so. The proprietary gallery build has a more advanced photo and video editor, while the foss one has a basic only.

If you try fixing a bug or adding a new feature, you should make sure that it is already reported at the given repository and the report is open and marked as a Bug or Feature Request. If the given issue is closed, chances are that we are not interested in the given feature and your pull request will likely be rejected.

<p>&nbsp;</p> 

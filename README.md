# www.mhsengineering.club

The official site of the MHS Engineering Club.

Live Site: [http://www.mhsengineering.club/](http://www.mhsengineering.club/)

# Contributing

All members of engineering club are free to contribute to the MHS Engineering
Club website. When contributing, we want the repository to stay as neat and
clean as possible, so please keep in mind the following rules:

- **Commit using pull requests.** If you want to commit, create a branch and
  request for the branch to be merged onto master. Don't try to commit directly
  to master.
- **Use spaces for indentation.** Set your editor to indent using spaces. Don't
  use tabs.
- **Write descriptive commits.** A good commit makes one clear change. Your
  commit message should describe what that change was and your description
  should describe why that change was made. Make sure you reference related
  issues.
- **Don't put images in the repository.** Putting images in the repository
  makes it needlessly larger.
- **Test before committing.** Don't commit anything you haven't tested
  yourself. Make sure to check all pages that could be affected by your
  change. For instance, if you alter `style.css`, you must check every html
  page that links to `style.css`.
- **Don't rely on /page to link to /page.html.** Github supports it, but most
  servers don't. If the file is at `/about.html`, link to `/about.html`. If you
  need a file to appear as `/about/`, put it at `/about/index.html`. We don't
  want to complicate testing environments by using nonstandard features.

## How to test

The easiest way to test is probably through the [Cloud9 IDE](https://c9.io/)
as it works on Chromebooks as well.  Set up a new workspace and "clone" this
repository, then `git checkout` the branch that you were working on.  Preview your
work by selecting the "Preview" button near the top of the page.
`git commit -am "Commit message here"` to commit your work, and then `git push` to
update it on Github.  To update, `git pull`.

Alternatively, if you have the HTML and CSS files on your computer already, simply
double-click the HTML file you want and reload it each time you make a change.  On
a Chromebook downloading the files is as easy as making sure you're on the correct
branch and then clicking the "Download ZIP" button on the right-hand side.

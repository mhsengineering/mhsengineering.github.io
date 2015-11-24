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

Testing will require you to run a server environment from your computer. This
is actually really easy and, once set up, can be started in seconds. Below are
some simple solutions to get you started.

Python provides an HTTP module that will run a simple HTTP server from the
current directory. This is started differently depending on what version of
python you're using.

    $ python2 -m SimpleHTTPServer
    Serving HTTP on 0.0.0.0 port 8000 ...
    127.0.0.1 - - [20/Nov/2015 13:52:10] "GET / HTTP/1.1" 200 -
    (^C to stop)
    $ python3 -m http.server
    Serving HTTP on 0.0.0.0 port 8000 ...
    127.0.0.1 - - [20/Nov/2015 13:54:00] "GET / HTTP/1.1" 200 -
    (^C to stop)

If you don't have python, [devd](https://github.com/cortesi/devd) is
a lightweight tool that also provides a simple HTTP server.

    $ devd .
    13:56:44: Listening on http://devd.io:8000 (127.0.0.1:8000)
    13:57:00: GET /
      <- 200 OK 2.8kB

If you're on a device that can't support a test environment, options are
available for remote environments. [Cloud9 IDE](https://c9.io/) provides an
online Linux environment that works on most browsers (ex. Chromebooks).

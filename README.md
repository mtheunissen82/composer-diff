composer-diff
=============

`composer-diff` performs a `git diff` command on your project.

Unlike `git diff`, however, it will also return differences in any packages marked in your composer.lock file

Usage
-----

    composer-diff diff sha-from [sha-to]

 * `sha-from` is the SHA of your project to use as the starting point
 * `sha-to` is the SHA of your project to use as the end point. If ommitted, the current check-out of code is used

Limitations
-----------

 * Doesn't work if a package isn't checked out in your project as a git repo
 * Output not the best
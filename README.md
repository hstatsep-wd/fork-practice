# Directions:
1. Fork this repo by clicking **Fork** in the top-right corner. Awesome, now you know how to fork. All of the directions below are just other cool things you can do with Git & Github.
2. Now that you have your own copy, go into the repo settings (gear icon) and rename your copy to `forking-practice`.
3. Clone your remote copy into your local IDE.
4. Make a new directory in this repo named `subdir`
5. READ what your command line says back to you when you try to add/commit/push!
6. Since we can't commit an empty directory, `cd` into `subdir` and create a file named `ready.txt`. Go ahead and put some text in that file: it can be whatever you want. But hold on, don't commit yet.
7. Go back up one level to the top-level directory by doing `cd ..` and make a file named `notready.txt`.
8. Use `git status` to see that both `notready.txt` and `subdir/` are in red (_really_, `subdir/` in this case means `subdir/notready.txt`).
9. While we typically use `git add .` to add _everything_ to the stage, let's imagine that `subdir/ready.txt` is ready to be committed, but `notready.txt` isn't. So try `git add subdir/ready.txt` to make sure that we add _only_ that file to the stage, and _NOT_ `notready.txt`.
10. Do `git status` again to confirm that `subdir/ready.txt` is green, and `notready.txt` is red.
11. Go ahead and commit, then push!
12. If you haven't already, reload your fork on GitHub. You should see your changes, except for `notready.txt`.
13. One last thing. You know how you can see the exact changes in commits by looking at them on Github? [Here is an example](https://github.com/hstatsep-wd/fork-practice/commits/main). But what about local changes that haven't been committed yet: how do we know what we've done locally before we commit and push them to Github? After all, this would probably help us come up with a good commit message ("wait... what did I do since my last commit?"). To show you, go ahead and change some text in your `subdir/ready.txt` file: again, it can be whatever you want. Now in your terminal, type `git diff` to see what you've changed since your last commit. Pretty cool, eh? Go ahead and add/commit/push _JUST_ that file again (`notready.txt` is still not ready).

That's it, you're done!

To recap, we saw that:
* You can't commit an empty directory.
* You can add just _some_ things to the stage, and thus not commit everything.
* You can see any new _uncommitted_ local changes by doing `git diff`.

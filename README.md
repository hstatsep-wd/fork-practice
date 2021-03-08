# Directions:
1. Fork this repo by clicking **Fork** in the top-right corner. Awesome, now you know how to fork. Everything 
2. Once your have your own copy, go into the repo settings and rename your copy to `forking-practice`.
3. Clone your remote copy into your local IDE.
4. Make a new directory named `subdir`
5. READ what your command line says back to you when you try to add/commit/push!
6. Since we can't commit an empty directory, `cd` into `subdir` and create a file named `ready.txt`. But hold on, don't commit yet.
7. Go back up one level to the top-level directory and make a file named `notready.txt`.
8. Use `git status` to see that both `notready.txt` and `subdir/ready.txt` are in red.
9. While we typically use `git add .` to add _everything_ to that stage, let's imagine that `subdir/ready.txt` is ready to be committed, but `ready.txt` isn't. So try `git add subdir/ready.txt` to make sure that we add _only_ that file to the stage, and _NOT_ `notready.txt`.
10. Do `git status` again to confirm that `subdir/ready.txt` is green, and `notready.txt` is red.
11. Go ahead and commit, then push!
12. If you haven't already, reload your fork on GitHub; you should see your changes, but no `notready.txt`.

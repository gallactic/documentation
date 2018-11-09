Contributions
=============
Help is always appreciated! Thanks for considering making contributions to Gallactic!

Please follow standard github best practices: fork the repo, branch from the tip of develop, make some commits, and submit a pull request to develop. Look at the `open issues <https://github.com/gallactic/gallactic/issues>`_ for things we need help with!

Forking
-------
Please note that Go requires absolute paths. So to work on a fork of gallactic, 
you have to still work in ``$GOPATH/src/github.com/gallactic/gallactic``. But you can add your fork as a new remote to work within same directory as gallactic project. For instance, to work on a new branch from b00f fork, You should would:

:: 

    cd $GOPATH/src/github.com/gallactic
    git clone https://github.com/gallactic/gallactic/
    cd galalctic
    git remote add b00f https://github.com/b00f/gallactic
    git fetch origin
    git checkout -b mybranch origin/develop

Now you will have the branch mybranch from b00f fork at ``github.com/b00f/gallactic`` checked out, 
but locally it's in ``$GOPATH/src/github.com/gallactic/gallactic``, rather than ``$GOPATH/src/github.com/b00f/gallactic``, which should actually never exist.

Now you can make changes, commit, and push to b00f fork:

Pull request
------------
Before sending pull request make sure you rebase your branch on develop branch. Also please make sure to use ``make fmt`` before every commit.

:: 

    < make some changes >
    make fmt
    git add -a
    git commit -m "... some messgae ..."
    git fetch origin
    git rebase origin/develop
    git push b00f

Now you can make a Pull Request.
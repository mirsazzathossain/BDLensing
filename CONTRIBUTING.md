## How to provide updates to the main repository

This document will guide you how to provide updates to the BDLensing 
repository through a pull request.

## Fork the repository

1. Go to main GitHub page of this repository.
2. Click on the "Fork" button on the top-right corner of the page.
3. Choose the account or organization where you want to fork the repository.

## Clone the forked repository
1. Go to your forked repository on GitHub.
2. Click on the "Code" button and copy the repository URL.
3. Open your terminal or Git Bash.
4. Change the current working directory to the location where you want to 
   clone the repository. 
5. Type `git clone <URL>`, where `<URL>` is the forked repository's URL, to 
   clone the repository to your local machine.

## Add upstream remote
1. Navigate to the cloned repository in your terminal.
2. Type `git remote -v` to view your remote repositories.
3. Verify that your forked repository is listed under "origin".
4. Copy the URL of the main repository.
5. Type `git remote add upstream <main repository URL>` to add the main 
   repository as an upstream remote.
6. Type `git remote -v` to verify that the upstream repository has been added.
7. Add the main repository as an upstream remote using `git remote add 
   upstream 
   <URL>`, where `<URL>` is the repository's URL.

You only need to do the above steps once. After the first-time setup, you can 
skip to the next section each time you want to make changes to the code. At this point,
you should check out [REVIEWING.md](https://github.com/ajshajib/BDLensing/blob/main/REVIEWING.md) 
to learn about what would be checked during the review of your code after 
you have created a pull request.

## Make changes and commit
1. Make changes to the code in your local clone of your fork.
2. Stage the changes using `git add .`
3. Commit the changes using `git commit -m "<commit message>"`. The 
   first word of the commit message should be a verb in the present form. 
   For example, "Modify mask for DESIJ0123" or "Update lens model 
   for DESIJ2376".

## Push changes to your forked repository on GitHub
1. Pull from upstream using `git pull upstream main`.
2. **Never do `git push upstream main`.** This will push your changes to the 
   main repository, which is not what you want to do.
3. Fix any merge conflicts. There should not be any merge conflicts, if 
   everyone is modifying only the files for their own lens systems.
4. Push the changes to your forked repository on GitHub using `git push origin main`.

## Send a pull Request to the main repository
1. Go to the original repository on GitHub.
2. Click on the "New pull request" button.
3. Choose the main branch in your forked repository as the "compare" branch 
   and the main branch in the original repository as the "base" branch.
4. Review the changes and **add a description**. Example descriptions are, "This PR updates 
the modeling notebook with progress made.", "Initial mask is created, this PR intends 
to close #<issue_number>", or "Optimization of initial model with PSO is completed 
for <Lens_Name>. This PR intends to close #<issue_number>".
6. Click on the "Create pull request" button to send the pull request to the 
   main repository.

That's it! Your changes will be reviewed, and if they are 
accepted, they will be merged into the main repository.

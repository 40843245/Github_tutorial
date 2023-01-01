# Objectives
In this article, I will teach you:
How to mirror repos in GitHub?
# method
method 1:
To mirror a repos with a few files to another repos, you can do
Step 1:
Open Git Bash.
Step 2:
Create a bare clone of the repos you want to copy.
Such as
git clone --bare https://github.com/EXAMPLE-USER/OLD-REPOSITORY.git
Step 3:
Mirror-push to the new repos.
Such as 
cd OLD-REPOSITORY.git
git push --mirror https://github.com/EXAMPLE-USER/NEW-REPOSITORY.git
Step 4:
Remove the temporary local repos you created earlier.
Such as
cd ..
rm -rf OLD-REPOSITORY.git

method 2:
Step 1:
Open Git Bash.
Step 2:
To create a bare clone of the repos you want to copy, type
git clone --bare
Such as
git clone --bare https://github.com/EXAMPLE-USER/OLD-REPOSITORY.git
Step 3:
Navigate to the repos you just cloned.
cd OLD-REPOSITORY.git
Step 4:
To pull in the repos's Git Large File Storage objects, type
git lfs fetch --all
Step 5:
To mirror-push to the new repos, type
git push --mirror
Such as
git push --mirror https://github.com/EXAMPLE-USER/NEW-REPOSITORY.git
Step 6:
To push the repos's Git Large File Storage objects to your mirror, type
git lfs push
Such as
git lfs push --all https://github.com/EXAMPLE-USER/NEW-REPOSITORY.git
Step 7:
Remove the temporary local repos you created earlier.
cd ..
rm -rf OLD-REPOSITORY.git

# Ref
https://docs.github.com/en/repositories/creating-and-managing-repositories/duplicating-a-repository

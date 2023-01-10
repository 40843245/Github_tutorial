# Objectives
How to rename a codespace for GitHub?

# Method
## method 1 (In GitHub)
Step 1:
Sign in GitHub with your account.

Step 2:
Click "Codespaces" button(at the middle of top menu).

Step 3:
Click "all codespace" button to list all available codespace.

You can alternatively either click the link or copy and paste the link instead of step 2. and step 3.
https://github.com/codespaces

Step 4:
Select your codespace.

Step 5:
Nagivate to "..." and select "rename" in menu bar.

Step 6:
Fill in information.

Step 7:
Click "ok" button.

<img src="https://github.com/40843245/Github_tutorial/blob/main/CodeSpace/Rename/RenameCodespace1.jpg">

## method 2 (using GitHub CLI)
Step 1:
Check you login. If you don't login, please login first.

Step 2:
Check the scope codespace has enough permission.
If NOT, please give it permission first.
You can use the following command in terminal.
gh auth refresh -h github.com -s codespace

Step 3:
To see all available codespace in terminal, type the command.
gh codespace list

NOTE:
NOTE that if there is NOT enough permission in the scope "codespace", then there are exceptions in terminal.
In this case, you have to use the above command to give permission.

Step 4:
To rename of codespace in terminal, type the following command.
gh codespace edit -c <PERMANENT-CODESPACE-NAME> -d <NEW-DISPLAY-NAME>
where
<PERMANENT-CODESPACE-NAME> indicates the permant name for codespace.
<NEW-DISPLAY-NAME> indicates that you want to change the codespace to <NEW-DISPLAY-NAME>.


# Ref
## See all available codespace
https://github.com/codespaces
## GitHub Docs
https://docs.github.com/en/codespaces/customizing-your-codespace/renaming-a-codespace


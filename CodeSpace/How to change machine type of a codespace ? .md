# Objectvies
How to change machine type of a codespace ?
# Method
## method 1 (in GitHub):
Step 1: Sign in GitHub with your account.

Step 2: Click "Codespaces" button(at the middle of top menu).

Step 3: Click "all codespace" button to list all available codespace.

You can alternatively either click the link or copy and paste the link instead of step 2. and step 3. https://github.com/codespaces

Step 4: Select your codespace.

Step 5: Nagivate to "..." and select "change machine type" in menu bar.

Step 6: Select the option.

Step 7: Click "ok" button.

## method 2 (using GitHub CLI):

Step 1: Check you login. If you don't login, please login first.

Step 2: Check the scope codespace has enough permission. If NOT, please give it permission first. 
You can use the following command in terminal. 
gh auth refresh -h github.com -s codespace

Step 3: To see all available codespace in terminal, type the command. 
gh codespace list

NOTE: NOTE that if there is NOT enough permission in the scope "codespace", then there are exceptions in terminal. In this case, you have to use the above command to give permission.

Step 4: To rename of codespace in terminal, type the following command. 
gh api </user/codespaces>/<CODESPACE-NAME>
where 
 <CODESPACE-NAME> indicates the permant name for codespace which indicates that you want to change settings of <CODESPACE-NAME>".

</user/codespaces>/<CODESPACE-NAME> indicates the relative path or absolute path.
   
# Ref:
## GitHub Docs
https://docs.github.com/en/codespaces/customizing-your-codespace/changing-the-machine-type-for-your-codespace?tool=webui
 
 https://docs.github.com/en/codespaces/customizing-your-codespace/changing-the-machine-type-for-your-codespace?tool=cli

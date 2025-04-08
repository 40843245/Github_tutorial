# How to Git control for a project in VS and create a Git repo in GitHub?
## Answer
### Prequisite
1. Stable Connection.
2. Patience.
   
### Step
Step 1:

Select `Git commits` tab.

Step 2:

Then click `build Git Repo` in `Git commits` tab.

<img width="959" alt="image" src="https://github.com/user-attachments/assets/b75f36cb-25b2-4961-ae30-ac7bd0e73041" />

Step 3:

If you have signed in yet, sign in GitHub account and grant permission of GitHub account to Visual Studio.

> [!NOTE]
> You can sign in GitHub account and grant permission of GitHub account to Visual Studio by click the dropmenu highlighted in red line.
> 
> <img width="551" alt="image" src="https://github.com/user-attachments/assets/12ee8477-88fb-4a4b-9ce8-35c044c9d98c" />

Step 4:

Ensure the configuration. Including 

| configuration | editable | description |
| ----------- | --------- | --- |
| `Local machine path` | editable | What project will commit and push to GitHub repo (determined by its full path) |
| `Account` | selectable | Which GitHub account will be committed and pushed to |
| `Owner` | selectable  | Which owner in GitHub account will be committed and pushed to |
| `Repo name` | editable | The name of committed and pushed repo. It will build a Git repo named `Repo name` |
| `Description` | editable | The description of the repo |
| `Private Repo` | tickable | The built Git repo will be private or not. If ticked, it is set to private. Otherwise, it is set to public (i.e. any with link can see it). | 
| `Repo url` | non-editable | the url of the built Git repo. As it consists of `Account` and `Repo name`, it is non-editable, you just have to check it correct (although it should be correct) |

![image](https://github.com/user-attachments/assets/e3c6d027-2e80-4a57-82a4-cb65e4b89d37)

Step 5:

Then click `commit and push` button.

Step 6:

Take a few minutes.

Step 7:

Check the repo is built.


To check the repo is built

1. first, go back to VS to see it finishes to build the Git repo.
  
2. If finishes to build the Git repo, go back to GitHub with that GitHub account.

> [!WARNING] 
> **NEVER** reload the web page in GitHub to make any changes in GitHub take effect.

## demo
See [Demo of git control for a project in VS and create Git repo in Github?](https://youtu.be/FR8kT1qm37o)

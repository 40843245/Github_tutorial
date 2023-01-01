# Objectives
In this article, I will teach you:
How to create a repos of GitHub using curl in Git Bash?
# Preparation
Check the curl is installed.
# method
Step 1:
Open Git Bash.
Step 2:
Type such as  

 curl \
  -X POST \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <Your Token>"\
  https://api.github.com/user/repos \
  -d '{"name":"Hello-World","description":"This is your first repo!","homepage":"https://github.com","private":false,"is_template":true}'

where
(2.1)The argument -d refers description of the repository. It only accept JSON type.
In argument -d, "name" refers the name of repository, "description" refers the description of the repository,
"private" refers the access privilege is private or NOT.
  
(2.2)The argument -H refers the the header of the host.
  
For example,
To send the header X-you-and-me: yes to the server when getting a page:
curl -H "X-you-and-me: yes" www.love.com

(2.3)The argument -X, --request <method>
will use the <method> method to handle server requests.
  
<img src="https://github.com/40843245/Github_tutorial/blob/main/Basic%20Operation/Repos/Create%20Repos/CurlMan1.png">

# Ref
(1)How to create a repository of GitHub in Git Bash?
https://docs.github.com/en/rest/repos/repos?apiVersion=2022-11-28#create-a-repository-for-the-authenticated-user
(2)Docs of curl.
https://curl.se/docs/manual.html
https://curl.se/docs/manpage.html

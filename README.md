# rml_calendar
Remote repo for the rainmanland.com self-scheduling and route optimization web app

## The code pipeline
cPanel uses something called **Pull Deployment** to handle the code pipeline. With pull deployment, each team member pulls from and pushes to a remote repository hosted outside of cPanel (GitHub in our case).

cPanel has its own clone of the GitHub repo in `~/repositories/rml_calendar`. When we want to pull changes from GitHub to the cPanel repo, we follow these steps:
1. Go to the cPanel dashboard
2. Go to the Git Version Control section of the dashboard
3. Click "Manage" next to the repository name
4. Click "Update from Remote" to pull updates from the GitHub repo to the cPanel repo
5. Click "Deploy HEAD Commit" to deploy the changes to the live site
![illustration of pull deployment](https://docs.cpanel.net/img/git-pull-deployment-workflow.png)

See [this article](https://docs.cpanel.net/knowledge-base/web-services/guide-to-git-how-to-set-up-deployment/) for more information on pull deployment.

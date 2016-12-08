# Wordpress-Git-Private-Plugin-Updater
Release Wordpress private/commercial plugin updates with git.

# Current state

This is atm just an idea. If I have enough time and keep up with my passion I will develop this.

# Intention

You've invested alot of work to develop a plugin for a client or for your company. Of cause you've used git while developing this plugin. Now you've the plugin installed manually in a wordpress installation, probably version 1.0 - but there is a bug - you need to hotfix it! So just update the code, push it to your gitrepo `git commit -m"Hotfix #1"`, download the zip and install it manually? No - this is so 2009, we're living in the era where we automate everything.

And I couldn't find anything that is good and easy enough to use, so this idea got out of my idea book in to this repo.

So this is the plan:

1. Wordpress-Plugin is in a private (or public) GitHub repository
2. You update your plugin frequently
3. You release a new version with a [`tag`](https://git-scm.com/book/en/v2/Git-Basics-Tagging)
4. This script here is installed as a cronjob on your server or a local NAS and checks the GitHub API for new tags and releases an update (generates a zip file, places it somewhere your wordpress page can download it) - Maybe this would be also more comfy by using webhooks.
5. The snippet (for your plugin) will be also here available, so your plugin know where to check for updates and where to download it
6. And the plugin get's a classic update (like with offical plugins)

# Development Progress
- [ ] Basic Plan (Flowchart)
- [ ] File structure
- [ ] Cronjob
- [ ] Adapter for GitHub
- [ ] Adapter for GitLab
- [ ] Adapter for BitBucket
- [ ] Adapter template for a new system?
- [ ] Codesnippet for the plugin
- [ ] Installation docs
- [ ] Usage docs
- [ ] first Alpha version

_Related: http://wordpress.stackexchange.com/q/13/75169_

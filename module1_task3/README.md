#Introduction to DevOps: Automate Everything to Focus on What Really Matters

## Prerequisites
* Install Go-Hugo
* There are no Git Submodules
* The theme ananke is installed
* Makefile present

## Lifecycle
* build: Generate the website from the markdown and configuration files in the directory dist/
* clean: Cleanup the content of the directory dist/
* post: Create a new blog post whose filename and title come from the environment variables POST_TITLE and POST_NAME
* help: Print out the list of target's usage
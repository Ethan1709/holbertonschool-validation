build:
		hugo

clean:
		rm -rf dist/*

post:
		hugo new posts/$(POST_NAME).md
		sed -i 's/title: .*/title: "$(POST_TITLE)"/' content/posts/$(POST_NAME).md

help:	## Show this help.
		@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\\$$//' | sed -e 's/##//'
.PHONY: build clean post

build:
    hugo -d dist/

clean:
    rm -rf dist/*

post:
    hugo new posts/$(POST_NAME).md
    sed -i '1s/^/---\ntitle: "$(POST_TITLE)"\n---\n/' content/posts/$(POST_NAME).md
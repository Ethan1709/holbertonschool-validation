build: ##compile the source code of the application to a binary name
	golangci-lint run
	go build
run: ##Run the application in background by executing the binary awesome-api
	./awesome-api >./awesome-api.log 2>&1 &
stop: ##Stop the application with the command kill XXXXX where XXXXX is the Process ID of the application
	pkill awesome-api || true
clean: ##Stop the application. Delete the binary awesome-api and the log file awesome-api.log
	pkill awesome-api || true
	rm -f awesome-api awesome-api.log coverage-*
test: ##execute all the tests
	go test -v -short -coverprofile=coverage-units.out
	go test -v -coverprofile=coverage-integrations.out
lint: ##Fail when the linter catches and error
	golingci-lint run
post: ##add a new post
	go test -v -coverprofile=coverage-integrations.out
check: ##check for something
	go test
help: ##help for user
	@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\
\\$$//' | sed -e 's/##//'
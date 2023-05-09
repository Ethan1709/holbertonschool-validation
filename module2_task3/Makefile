build: ##compile the source code of the application to a binary name
	golangci-lint run
	go build
run: ##Run the application in background by executing the binary awesome-api
	./awesome-api >./awesome-api.log 2>&1 &
stop: ##Stop the application with the command kill XXXXX where XXXXX is the Process ID of the application
	pkill awesome-api || true
clean: ##Stop the application. Delete the binary awesome-api and the log file awesome-api.log
	pkill awesome-api || true
	rm awesome-api awesome-api.log
test: ##You want to test it to ensure that it behaves as expected
	curl http://localhost:9999
	curl http://localhost:9999/health
lint: ##Fail when the linter catches and error
	golingci-lint run
unit-tests: ##should execute (successfully) the Golang unit tests
	go test -v -short -coverprofile=coverage-units.out
intgration-tests: ##integration test
	go test coverage-integrations.out
help: ##help for user
	@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\
\\$$//' | sed -e 's/##//'
build: ##compile the source code of the application to a binary name
	go build
run: ##Run the application in background by executing the binary awesome-api
	./awesome-api >./awesome-api.log 2>&1 &
stop: ##Stop the application with the command kill XXXXX where XXXXX is the Process ID of the application
	pkill awesome-api
clean: ##Stop the application. Delete the binary awesome-api and the log file awesome-api.log
	pkill awesome-api
	rm awesome-api awesome-api.log
test: ##You want to test it to ensure that it behaves as expected
	curl http://localhost:9999
	curl http://localhost:9999/health
help: ##help for user
	@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\
\\$$//' | sed -e 's/##//'
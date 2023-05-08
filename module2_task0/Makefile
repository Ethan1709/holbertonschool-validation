build:
	go build
run:
	./awesome-api >./awesome-api.log 2>&1 &
stop:
	kill "$(pgrep awesome-api)"
clean:
	kill "$(pgrep awesome-api)"
	rm awesome-api awesome-api.log
test:
	curl http://localhost:9999
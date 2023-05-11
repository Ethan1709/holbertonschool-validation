## Testing in the Software Development Methodology

### Prerequisites
* Golang in v1.15.*
* NPM v7+ with NodeJS v14.* (stable)
* Python 3 with pip module
* golangci-lint

### Lifecycle
* "build": compile the source code of the application to a binary
* "run": Run the application in background by executing the binary
* "stop": Stop the application with the command kill XXXXX where XXXX\
X is the Process ID of the application
* "clean": delete all the generated files
* "test": You want to test it to ensure that it behaves as expected
* "help": Print a list of all the goals with a sentence
* "lint": Fail when the linter catches and error
* "test": should execute all the tests
* "post": add a new post
* "lint": Fail when the linter catches and error
* "check": Succeed by default, and fail when presented with a dead link or a badly written Markdown file
* "validate": Always succeed by default and should print the result on the stdout
* "unit-tests": should execute (successfully) the Golang unit tests
* "integration-tests": making integration tests
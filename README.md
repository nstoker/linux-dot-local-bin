# linux-dot-local-bin

Some random scripts I find helpful.

## Container scripts

Script      | Purpose
------------|---------
`generic`   | Start and stop a container `generic`. Copy this file to the name of a container to get start, stop, status, and restart commands. It checks for the name of the file being executed using `basename $0`.
`postgres`  | Starts and stops the postgres service. Options are: `start`, `stop`, `status`, and `restart` commands.

### Golang related

Script           | Purpose
-----------------|---------
`start-go`       | Checks if the directory contains a go.mod file, then starts code, go-convey, and git cola running.
`start-goconvey` | Starts the goconvey test runner app in a new terminal. This will also open a browser widow showing the results of the test runner.

#### Ruby on Rails related

Script           | Purpose
-----------------|--------
`start-guard`    | If the Guardfile is present in the current directory, then starts the guard service in a new terminal.
`start-rabbitmq` | If the `docker-compose-rabbit.yml` exists, then starts the rabbitmq services. TODO: Can this be replaced by a generic container script.
`start-rails`    | If the Gemfile is present in the current directory, then starts code, start-guard, and git cola.
properties([
	pipelinetriggers([pollSCM('H/3 * * * *')]
	)]

node() {
	cleanWs()
	checkout scm
	sh"make"
	sh"./main"
}

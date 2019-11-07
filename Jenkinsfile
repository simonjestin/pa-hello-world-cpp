properties([
	pipelineTriggers([pollSCM('H/3 * * * *')])
	])

node() {
	cleanWs()
	checkout scm
	sh "make"
	sh "./main"
	archiveArtifacts artifacts: 'generatedFile.zip'
}

archiveArtifacts {
	artifacts:'toto.zip'
}

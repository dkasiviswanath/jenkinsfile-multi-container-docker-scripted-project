node{

        stage('build-java'){
		docker.image('maven:3-alpine').inside('-v $HOME/.m2:/root/.m2'){
                        sh 'mvn -v'
                }
        }
	
	stage('build-java-script-nodejs'){
                docker.image('node:7-alpine').inside{
                        sh 'node --version'
                }
        }
}

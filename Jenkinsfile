node {
        stage('Checkout') {
            git url: 'https://github.com/paramjeet13/SoapProject.git/my-app/',  branch: 'master'
            echo '****************CHECKOUT SUCCESSFUL****************'
        }
       

       
			
	stage('Build') {
		def mvn_version = 'Maven_Home'
		withEnv( ["PATH+MAVEN=${tool mvn_version}/bin"]) {
			sh 'mvn site'
			}
		}
}

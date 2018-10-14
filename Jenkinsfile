pipeline {
    agent any

    stages {
		
        stage ('Build Stage') {

            steps {
			dir("/root/.jenkins/workspace/pipeline9"){
			sh 'mvn clean install'
            }
            }
        }

        
		stage ('Deployment Stage') {

            steps {
                
                    sh 'cp /root/.jenkins/workspace/pipeline9/target/simple-web-app.war /opt/apache-tomcat-8.5.34/webapps '
              
            }
        }


        
    }
}

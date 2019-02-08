#!/usr/bin/env groovy 

// Jenkinsfile (Declarative Pipeline)
pipeline {
    agent any
    stages {
//        stage('checkout') {
//            steps {
//				echo "Checking out Declarative ${env.JOB_NAME}"
//				git branch: 'master', credentialsId: 'KyleFinley1', url: "https://github.com/KyleFinley1/helloJava.git"
//            }
//        }
        stage('build') {
            steps {
				echo "Building Declarative ${env.JOB_NAME}"
                // sh 'mvn --version'
                // bat 'C:\Program_Files_COTS\Java\jdk1.8.0_191\bin\javac.exe C:\Program_Files_COTS\Jenkins-2.150.2\workspace\helloJava\helloJava.java'
				// bat 'set JAVA_HOME=C:\\Program_Files_COTS\\Java\\jdk1.8.0_191\\bin\\'
				// bat "%JAVA_HOME%javac.exe %WORKSPACE%\\helloJava.java"

                bat 'C:\Program_Files_COTS\Java\jdk1.8.0_191\bin\javac.exe %WORKSPACE%\\helloJava.java'
				// bat "build.bat"
            }
        }
    }

//    post {
//        failure {
//            echo "${env.JOB_NAME} pipeline failed :("
//          // Needs SMTP port 25 available or Jenkins SMTP server assigned smtp.linquest.com
//			mail to: 'Kyle.Finley@LinQuest.com',
//				subject: "${env.JOB_NAME} pipeline failed :(",
//				body: "Something is wrong with ${env.BUILD_URL}"
//        }
//    }
}

// Jenkinsfile (Scripted Pipeline)
//node {
//    stage('build2') {
//			echo "Building Scripted ${env.JOB_NAME}"
//    }
//}

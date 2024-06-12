pipeline {
    agent any

    tools {
        maven 'Maven 3.9.6' // Name der Maven-Installation in der Global Tool Configuration
    }

    stages {
        stage('Checkout') {
            steps {
                // Code aus dem Versionskontrollsystem abrufen
                git 'https://github.com/your-repo/hello-world.git'
            }
        }

        stage('Build') {
            steps {
                // Führen Sie den Maven-Befehl aus
                bat 'mvn clean package'
            }
        }

        stage('Run') {
            steps {
                // Führen Sie das Java-Programm aus
                bat 'java -cp target/hello-world-1.0-SNAPSHOT.jar com.example.HelloWorld'
            }
        }
    }
}

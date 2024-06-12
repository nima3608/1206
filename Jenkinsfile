pipeline {
    agent any

    tools {
        maven 'Maven 3.9.6' // Name der Maven-Installation in der Global Tool Configuration
    }

    stages {
        stage('Build') {
            steps {
                // Wechseln Sie in das Verzeichnis, das die pom.xml-Datei enthält
                dir('path/to/your/project') {
                    // Führen Sie den Maven-Befehl aus
                    bat 'mvn clean package'
                }
            }
        }
    }
}

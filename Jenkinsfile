pipeline {

    options {
        // Build auto timeout
        timeout(time: 60, unit: 'MINUTES')
    }
    // Pipeline stages
    agent { node { label 'master' } }
    stages {

        ////////// Step 1 //////////
        stage('Apply k8s-manifests') {
            steps {
                echo "Apply k8s-manifests"
                sh "kubectl apply -f ."
            }
        }
    }
}
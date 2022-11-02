pipeline {

    options {
        // Build auto timeout
        timeout(time: 60, unit: 'MINUTES')
    }
    // Pipeline stages
    stages {

        ////////// Step 1 //////////
        stage('Apply k8s-manifests') {
            steps {
                echo "Apply k8s-manifests"
                kubectl apply -f .
            }
        }
    }
}
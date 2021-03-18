node {
    docker.image("gradle:latest").inside() {
        stage('Checkout') {
            git 'https://github.com/gantta/RestaurantList.git'
        }
        stage('Build') {
            sh 'gradle clean build'
        }
        stage('Code Quality') {
            echo 'Skipping sonarqube b/c fuck it'
            //sh 'gradle sonarqube -Dsonar.projectName=SimpleGreetingGradle -Dsonar.projectKey=SimpleGreetingGradle -Dsonar.host.url=http://192.168.4.74:9000 -Dsonar.login=673257e155348e0c22c0d6c03a83c757161e4c78'
        }
    }
}
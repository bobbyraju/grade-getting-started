node {
    stage('Preparation') {
        git 'https://github.com/bobbyraju/grade-getting-started.git'
    }
    stage('Build') {
        sh "./gradlew clean test"
    }
    stage('Deploy') {
        sh "git push https://git.heroku.com/pure-cliffs-85232.git master"
    }
}
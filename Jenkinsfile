properties([parameters([choice(choices: 'main\nfeature1\nfeature2', description: 'Select a branch to build', name: 'branch')])])
node {
    stage('SCM checkout') {
        echo "Pulling changes from the branch ${params.branch}"
        git url: 'https://github.com/riyag283/java-app', branch: "${params.branch}"
    }
    stage('Build') {
        steps {
            bat "javac App.java"
            bat "java App abcd"
        }
    }
}

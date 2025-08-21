node{
    git branch: 'main',  url: 'https://github.com/shrikov/simple-java-app.git'
    stage('build'){
        try{
            sh'echo "build app"'
        }
        catch(Exception e){
            sh'echo "error happened"'
            throw e
        }
        
    }
    stage('test'){
        if (env.Branch_name == "main"){
            sh'echo "branch name is main"'
        }
        else{
            sh'echo "skip test"'

        }
    }
}
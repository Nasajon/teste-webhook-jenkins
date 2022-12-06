node('aws-codebuild'){
    
    def build_num = currentBuild.number
    
    stage('Hello world'){
        echo "opa, joia?"
    }
    
    stage('post chat'){
        echo "postando no google chat"
        sh "curl -XPOST https://7f1a-187-95-168-12.sa.ngrok.io/webhook/${env.BRANCH_NAME}/${build_num}"
    }
}

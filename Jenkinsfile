node('aws-codebuild'){
    
    def build_num = currentBuild.number
    
    stage('Hello world'){
        echo "opa, joia?"
    }
    
    stage('post chat'){
        echo "postando no google chat"
        do_post("https://7f1a-187-95-168-12.sa.ngrok.io/webhook/${env.BRANCH_NAME}/${build_num}")
    }
}


def do_post(url){
    def postmanPost = new URL(url)
    def postConnection = postmanPost.openConnection()
    postConnection.requestMethod = 'POST'
    assert postConnection.responseCode == 200
}

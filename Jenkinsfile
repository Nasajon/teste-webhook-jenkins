node('master'){
    
    def build_num = currentBuild.number
    
    stage('Hello world'){
        echo "opa, joia?"
    }
    
    stage('post chat'){
        echo "postando no google chat"
        httpRequest httpMode: "POST", authentication: "${env.JENKINS_QUEBRADO}", url: "https://apisre.nasajonsistemas.com.br/webhook/Teste%20Webhook/${env.BRANCH_NAME}/${build_num}"
    }
}

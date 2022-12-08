node('master'){
    
    def build_num = currentBuild.number
    
    stage('Hello world'){
        echo "opa, joia?"
    }
    
    stage('post chat'){
        echo "postando no google chat"
        withCredentials([string(credentialsId: 'mytoken', variable: 'TOKEN')]) {
            httpRequest httpMode: "POST", authentication: "${TOKEN}", url: "https://apisre.nasajonsistemas.com.br/webhook/Teste%20Webhook/${env.BRANCH_NAME}/${build_num}"
        }
    }
}

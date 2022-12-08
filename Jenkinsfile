node('master'){
    
    def build_num = currentBuild.number
    
    stage('Hello world'){
        echo "opa, joia?"
    }
    
    stage('post chat'){
        echo "postando no google chat"
        withCredentials([string(credentialsId: 'JENKINS_QUEBRADO', variable: 'TOKEN')]) {
            httpRequest customHeaders: [[maskValue: true, name: 'apikey', value: "${TOKEN}"]], httpMode: 'POST', ignoreSslErrors: true, url: "https://apisre.nasajonsistemas.com.br/webhook/Teste%20Webhook/${env.BRANCH_NAME}/${build_num}"
        }
    }
}

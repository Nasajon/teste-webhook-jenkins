node('master'){
    
    def build_num = currentBuild.number
    def jenkinsNameJob = "Instalador"
    
    stage('Hello world'){
        echo "opa, joia?"
        echo "opa, joia?"
        echo "opa, joia?"
        echo "opa, joia?"
        echo "opa, joia?"
        echo "opa, joia?"
        sleep(time:5,unit:"SECONDS")
    }
    
    stage('teste de current result'){
        try{
            dir("zeca")
            sleep(time:5,unit:"SECONDS")
            echo "PARABAINS, pode pegar um biscoito no final do corredor a esquerda"
        }catch (e) {
            if(currentBuild?.result == "FAILURE"){
                echo "xiii faio"
            }else{
                currentBuild.result = "ABORTED"
                echo "que coisa feia, abortando!"
                throw e
            }
        }
    }
}

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
            if(currentBuild?.result == "FAILURE"){
                echo "xiii faio"
            }
    
            else if(currentBuild?.result == "SUCCESS"){
                echo "PARABAINS, pode pegar um biscoito no final do corredor a esquerda"
            }
        }catch (e) {
            currentBuild.result = "ABORTED"
            echo "que coisa feia, abortando!"
            throw e
        }
    }
}

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
        sleep(time:5,unit:"SECONDS")
        if(currentBuild.currentResult == "FAILURE"){
            echo "xiii faio"
        }

        else if(currentBuild.currentResult == "SUCCESS"){
            echo "PARABAINS, pode pegar um biscoito no final do corredor a esquerda"
        }

        else if(currentBuild.currentResult == "ABORTED"){
            
            echo "que coisa feia, abortando!"
            error("bip bip parando...")
        }
    }
}
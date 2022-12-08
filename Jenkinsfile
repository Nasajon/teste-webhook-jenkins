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
    }
    
    stage('teste de current result'){
        if(currentBuild.currentResult == "FAILURE"){
            echo "xiii faio"
        }

        else if(currentBuild.currentResult == "SUCCESS"){
            echo "PARABAINS, pode pegar um biscoito no final do corredor a esquerda"
        }

        else{
            currentBuild.result = "ABORTED"
            echo "que coisa feia, abortando!"
            error("bip bip parando...")
        }
    }
}
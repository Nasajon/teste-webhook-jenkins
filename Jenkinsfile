node('master'){
    
    def build_num = currentBuild.number
    def jenkinsNameJob = "Instalador"
    
    stage('Fetch') {
        timeout(time: 60, unit: 'SECONDS') {
            checkout scm
        }
    }
    
    stage('Hello world'){
        echo "opa, joia?"
    }
    
    stage('iterate over something'){
        dir('docs/'){
            def files = findFiles(glob: '**/*.html')
            for (file in files){
                echo """
                ${files[0].name}
                """
            }
        }
    }
}
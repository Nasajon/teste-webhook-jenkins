node('master'){
    
    def build_num = currentBuild.number
    def jenkinsNameJob = "Instalador"
    
    stage('Hello world'){
        echo "opa, joia?"
    }
    
    stage('iterate over something'){
        def files = findFiles(glob: 'docs/**/*.html')
        for (file in files){
            echo """
            ${files[0].name} ${files[0].path} ${files[0].directory} 
            ${files[0].length} ${files[0].lastModified}
            """
        }
    }
}
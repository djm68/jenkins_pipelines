#!groovy

node ("linux") {
    stage 'Build' {
        sh 'echo Building...'
    }
    
    stage 'Brick Tests' {
        sh 'echo Running Brick Tests...'
    }

    stage 'Wait and Rest' {
        sh 'sleep 5'
        sh 'echo resting...'
    }
}

stage 'Functional Tests' {
    parallel (
        "UPnP Suite" : { 
                         node ("linux") { 
                               sh 'echo UPnP Tests'
                           } 
                       },
        "CPU Tests" : { 
                         node ("linux") { 
                               sh 'echo UPnP Tests'
                           } 
                       }
              )
}

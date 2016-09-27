#!groovy

stage 'Build'
    echo 'Building...'

stage 'Brick Tests'
    echo 'Running Brick Tests...'

parallel (
    "stream 1" : { 
                     node { 
                           echo 'UPnP Tests'
                       } 
                   },
    "stream 2" : { 
                     node { 
                           echo 'UPnP Tests'
                       } 
                   }
          )

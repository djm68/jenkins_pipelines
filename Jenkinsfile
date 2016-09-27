#!groovy

node{
    stage 'Build'
        echo 'Building...'

    stage 'Brick Tests'
        echo 'Running Brick Tests...'

    parallel 'integration-tests':{
        node('mvn-3.3'){}
    }, 'functional-tests':{
        node('selenium'){}
    }
}


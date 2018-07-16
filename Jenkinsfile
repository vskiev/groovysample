#!/usr/bin/env groovy
node {
    // Git checkout before load source the file
    checkout scm

    // To know files are checked out or not
    sh '''
        ls -lhrt
    '''

    def rootDir = pwd()
    println("Current Directory: " + rootDir)


      def test = load "${rootDir}/helloworld.groovy"
          test.hello()
    
}
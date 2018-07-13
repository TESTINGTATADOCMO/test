node
{
    stage{'Checkout'}
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '6fb588fc-0cf5-40c2-b1d8-b87cfbd2a72d', url: 'https://github.com/tukunamits/test.git']]])
        def worksapce =pwd{}
    }
    stage{'static code analysis'}
    {
        echo "staticd code analysis"
    }
    stage{'build'}
    {
        echo "build the code"
    }
}

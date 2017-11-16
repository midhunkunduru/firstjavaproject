node("master")
{
    stage("Checkout")
{  
    sh 'echo $BRANCH_NAME'
}
    
    stage("Build")
    {
        echo "Sample build"
        build job: 'parameterjob1/master', parameters: [string(name: 'param1', value: '1'), string(name: 'param2', value: '2'), string(name: 'param3', value: '3'), string(name: 'param4', value: '4')]
    }

}

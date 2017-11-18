node("master")
    
{
  def a = "Version"
  def b = "Application" 
    stage("Checkout")
      {  
         
    //sh 'echo $BRANCH_NAME'
    echo "${a}"
    echo "${b}"
}
    
    stage("Build")
    {
        echo "Sample build"
        build job: 'parametertest/master', parameters: [string(name: 'Version', value: 'a'), string(name: 'Application', value: 'b')]
    }

}

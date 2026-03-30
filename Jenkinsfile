@Library('jenkins-shared-library')_ 

def configMap = [
    project : "roboshop",
    component : "payment"
]

if( !env.BRANCH_NAME.equalsIgnoreCase('main')){
    pythonEKSPipeline.call(configMap)
}
else {
    echo "Proceed with PROD process"
}

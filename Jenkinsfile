pipeline{
    agent any
    parmeters{
        choice(name: PRODUCT, choice: choices['_Please select the product', 'X1help', 'X2help', 'X3help'], description: '')
    }
    stages {
        stage('Verify product'){
            steps{
                script{
                    if (params.PRODUCT == '_Please select the product'){
                        echo "Error: no product choosen"
                        sh "exit 1"
                    }

                    if (params.PRODUCT == 'X1help'){
                        echo "X1 Help getting execute"
                    }

                    if (params.PRODUCT == 'X2help'){
                        echo "X2 Help getting execute"                        
                    }

                    if (params.PRODUCT == 'X3help'){
                        echo "X3 help getting execute"
                    }
                }
 
            }
        }


    }

}
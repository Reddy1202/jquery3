aws ecr get-login-password --region us-east-2 | sudo docker login --username AWS --password-stdin 339232133467.dkr.ecr.us-east-2.amazonaws.com
sudo docker build -t 339232133467.dkr.ecr.us-east-2.amazonaws.com/jquery-eks:$BUILD_NUMBER .
sudo docker push 339232133467.dkr.ecr.us-east-2.amazonaws.com/jquery-eks:$BUILD_NUMBER
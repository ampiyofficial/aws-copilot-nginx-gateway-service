
# Initialize Copilot APP and Environment

        - Clone: https://github.com/ampiyofficial/aws-copilot-nodeapp-microservice
        - cd to Repo 
        
        - copilot app init test-copilot-app
        - copilot env init --name test --profile default --app test-copilot-app

# Deploying Node App on AWS Copilot
        
        1. copilot svc init --name nodeapp --svc-type "Backend Service" --dockerfile ./nodeapp/Dockerfile

        2. copilot svc deploy --name nodeapp --env test

        3. copilot pipeline init
        4. copilot pipeline deploy

# Deploying NGINX Gateway Server on AWS Copilot

        - Clone: https://github.com/ampiyofficial/aws-copilot-nginx-gateway-service
        - cd to Repo 
        - copilot app init test-copilot-app OR (Copy Copilot Folder with .workspace file)

        1. copilot svc init --name nginx-gateway --svc-type "Load Balanced Web Service" --dockerfile ./nginx-gateway/Dockerfile

        2. copilot svc deploy --name nginx-gateway --env test

        3. copilot pipeline init
        4. copilot pipeline deploy




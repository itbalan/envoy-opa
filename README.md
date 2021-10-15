# envoy-opa
Envoy integration with Open Policy Agent (OPA)

# Pre-requisites
1. Docker Engine installed and running
2. Docker Compose installed
2. Build service-template spring boot application and copy the jar file from ./target folder to the folder envoy-opa
2. Build service-template-greeting spring boot application and copy the jar file from ./target folder to the folder envoy-opa

Step1: Open command prompt and go to the directory envoy-opa

Step2: Run the command to build envoy front-proxy, service-template and service-template-greeting images: docker-compose build --pull

Step3: Run the command to deploy envoy front proxy, OPA, service-template and service-template-greeting containers:: docker-compose up -d

Step4: Run the command to check the containers running (you should see 4 containers running): docker-compose ps

Step5: Run the command to check the log: docker logs -f {container name or process id} 





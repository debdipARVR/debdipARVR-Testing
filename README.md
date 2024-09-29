Running Application .
Open Terminal Navigate to Script folder.
Run following commands step by step.
docker build -t parallel-allure-test .
docker-compose up --build
allure generate ./allure-results-container1 ./allure-results-container2 ./allure-results-container3 -o ./merged-results --clean
allure serve ./merged-results

## Microfrontend Component two - product-list

### 1) Create react app
    npm install -g create-react-app
    create-react-app product-list
    cd product-list/
    npm start
    
### 2) To build transpiled and run the server
    npm run build
    npm run transpile
    npm run start:prod
    
### 3) To run the app inside the Docker image
    docker build . -t product-list
    docker run -t -e PORT=8080 -p 8080:8080 product-list
    
### 4) to setup heroku
    heroku create microfrontends-component-two
    git push heroku master
    heroku container:login
    heroku container:push web
    heroku open
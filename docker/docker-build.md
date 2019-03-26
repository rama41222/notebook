### Docker 

1. Tag an image
    ``` 
    docker tag SOURCE_IMAGE[:TAG] TARGET_IMAGE[:TAG]
    ```
2. Building the image
    ```
    docker build -t IMAGE[:TAG] .
    ``` 
3. Pushing the image into DockerHub
    ``` 
    docker push IMAGE[:TAG]
    ```

*Docker imagename should be your username/imagename:tag when you're pushing into the docker hub.*

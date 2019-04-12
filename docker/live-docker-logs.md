### Docker Logs

To view the logs of a Docker container in real time, use the following command:

* The -f or --follow option will show live log output.
    ```
    docker logs -f <CONTAINER_ID>
    docker logs $(sudo docker ps -aq --filter name=<CONTAINER_ID>)
    ```

## Choose an Application to Experiment on

=== "httpbin"
    
    A simple HTTP Request & Response Service.

    Run the [httpbin](https://httpbin.org) sample service from a separate terminal.
    ```shell
    docker rm httpbin && docker run -d --name httpbin -p 80:80 kennethreitz/httpbin
    ```
    You can also use [Podman](https://podman.io) or other alternatives to Docker in the above command.

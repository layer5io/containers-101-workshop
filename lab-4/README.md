# Docker 101 - Linux (Part 4): Container Monitoring
Now that you are running let’s monitor your containers.

Tech strategy team has developed a tool to monitor containers. More info about it can be found here:
https://github.com/solarwinds/containers/tree/master/cnpt



In the console for `node1` initialize Docker Swarm

    ```
    $ docker run -d --name swi-agent --privileged --net=host --restart always -v /var/run/docker.sock:/host/var/run/docker.sock -v /dev:/host/dev -v /proc:/host/proc:ro solarwinds/container-agent
    
    ```


    ```
    $ docker run -d --name swi-ui -p 80:80 -t solarwinds/container-ui
    ```

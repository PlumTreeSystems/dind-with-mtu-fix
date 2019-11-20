# Docker dind image with mtu fix

We were having issues fetching packages from some remote repositories via the composer package manager, we traced it down to have something to do with t he network and with the MTU setting.

Using a workaround provided by a [kind fellow](https://discourse.drone.io/t/docker-mtu-problem/1207/4) - we made an image that solved our issue (by extending the docker entrypoint script provided by the docker team that made the dind image).

# Docker hub
[Link](https://hub.docker.com/repository/docker/plumtreesystems/dind-with-mtu-fix)

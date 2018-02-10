# vpl_docker
Virtual Programming Lab Jail system execution server running on Docker.

[Original Project](http://vpl.dis.ulpgc.es/)


## Run VPL Jail Server

```shell
sudo docker run --rm --privileged -p 80:80 -p 443:443 -it --user root hthuwal/vpl_docker bash -c "service vpl-jail-system start; bash"
```
### Explanation
- *--rm* removes the container as soon as you exit it
- *--privileged* gives extended permission to docker (required for vpl service to start)
- *-p* publish containers port 80 to host port 80 (vpl jail server runs at port 80)
- *-it* to allocate a tty for the container process

## Image

https://hub.docker.com/r/hthuwal/vpl_docker/

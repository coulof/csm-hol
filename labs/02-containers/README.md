## 🐋 Containers overview

In this section we will quickly explore the use of containers.

## Run your first container

`podman` is a daemonless container engine Docker-compatible CLI. Everything below can be done with `docker`.

To make sure it works correctly, run the following command:
```bash
podman run -it --rm hello-world
```


Now let's try with your favorite linux distribution (for example Ubuntu):
```bash
podman run -it --rm ubuntu
```

>**NOTE:** Let's discuss what we see.

## Build your first container

To build a container, run the following command:
```bash
podman build -t myimage .
```

```bash
podman run -it --rm myimage
```

>**NOTE:** There are a lot more to learn. If you want to deep-dive I recommend you check : [https://container.training](https://container.training/intro-selfpaced.yml.html#1).

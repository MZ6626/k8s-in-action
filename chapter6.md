## Chapter 6
## Sharing disk storage between containers in the Pod

Auxiliary files for the emptyDir pod's example can be found [here](Chapter_6)

To build the image run
``` bash
$ docker build -t <your_name>/fortune .
$ docker push <your_name>/fortune
```
To create a Kubernetes' pod run
``` bash
$ kubectl create -f fortune-pod.yaml
$ kubectl port-forward fortune 8080:80
```

Test it from your localmachine
```bash
$ curl http://localhost:8080
You will obey or molten silver will be poured into your ears.
```

## Using a Git repository as the starting point for a volume

Auxiliary files for the gitRepo pod's example can be found [here](Chapter_6)

To build the image run
``` bash
$ docker build -t <your_name>/fortune .
$ docker push <your_name>/fortune
```
To create a Kubernetes' pod run
``` bash
$ kubectl create -f fortune-pod.yaml
$ kubectl port-forward fortune 8080:80
```

Test it from your localmachine
```bash
$ curl http://localhost:8080
<html>
<body>
Hello there.
</body>
</html>
```
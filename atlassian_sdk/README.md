# Atlassian SDK Image
## Usage
Run 

```docker run --name atlassdk -it -p 1990:1990 -v $PWD:/home/confi orlopau/atlassian-sdk /bin/bash```

in the directory you want to mirror to the container.

---
Later you can easily start and stop the container using
```docker start atlassdk```
and
```docker stop atlassdk```

Opening a new terminal session inside the container:


```docker exec -it atlassdk /bin/bash```

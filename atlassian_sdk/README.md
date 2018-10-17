# Atlassian SDK Image
## Usage
Run ```docker run --name atlassdk -it -p 1990:1990 -v $PWD:/home orlopau/atlassian-sdk /bin/bash```

---
Later you can easily start and stop the container using
```docker start atlassdk```
and
```docker stop atlassdk```

Opening a new terminal session inside the container:


```docker exec -it atlassdk /bin/bash```

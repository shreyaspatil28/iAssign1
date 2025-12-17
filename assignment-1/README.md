# **Docker File**
Docker pulls image through Nginx by using command : 

```bash
docker pull nginx
```
In this docker file we copy `index.html` and expose port `7000` on the system and accessing port `7070` on the host.
Image named `shreyas-site` was built using command : 

```bash
docker build -t shreyas-site
```
Now we run the container using command : 

```bash
docker run -d --name web -p 7070:7000 shreyas-site
```
The site can be tested by opening `http://localhost:7070` on a browser or using the curl command : 

```bash
curl http://localhost:7070
```
Now the container is stopped by using command : 

```bash
docker stop web
```
And then the container can be removed by using command :

```bash
docker rm web
```

# **index.html**
The title of the page is set as Shreyas Patil and suitable styling is done for fonts, background color and text aligning.

In the body is mentioned my name as heading and a short description underneath.

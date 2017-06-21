# Windows-Container-jenkinDotnet-2.66

to build images use this command :

docker build -t windows-jenkins-dotnet:2.66 .

to create new container use this command :

docker run --name jenkinsci -p 8080:8080 -p 50000:50000
--dns 8.8.8.8 -d windows-jenkins-dotnet:2.66

to get the initial admin password use this command :

docker logs jenkinsci

# Dockerized React Native

Want to develop a React Native application in a container avoiding all versioning hassles? Well, you've come to the right repository!

Here, we've orchestrated a docker container with a bare minimum React Native application with Expo managed workflow.

## pre-requisites

- docker
- docker-compose (which usually comes along with docker but if it's not the case then yeah)

## steps

- clone this repository using `git clone https://github.com/taher07/dockerized-react-native.git my-app`
- Navigate to the repository and run `rm -rf .git/`
- Run `docker-compose up`, you gotta give it some time
- Your React Native application would have probably been running by now, go to [http://0.0.0.0:19002](http://0.0.0.0:19002) from your browser and it would render dev tools in your browser
- Under the `connection` session click on `Tunnel` and you can now run your expo managed app from the Expo Go app on Android or iOS devices
- Now let's get into bash specific to docker container as
  - Run `docker ps` and copy the container id
  - Run `docker exec -it <container_id> bash`
- You're all set to start developing your dockerized React Native application

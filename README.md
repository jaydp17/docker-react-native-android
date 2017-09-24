# docker-react-native-android
A 🐳 docker image for building ⚛ React Native Apps (Android only)

### Installed Packages
- Open JDK 8
- Gradle v3.3
- Android SDK 23, 25 & 26
- Android Build Tools 23.0.1, 25.0.2, 26.0.1
- Android Tools (tools, platform-tools, extras)
- Google Extras

## How to use?
```sh
# The below will run the container and open up a bash session in side the container
$ docker run --rm -it -v /path/to/my/react-native-app:/app jaydp17/react-native:latest bash

# Now cd into the android folder and build the app
$ cd /app/android

# install npm modules
$ yarn

# build the app
$ ./gradlew assembleRelease
```

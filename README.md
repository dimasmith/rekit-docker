# rekit-docker
Docker container for awesome rekit IDE. Used to test docker auto builds

Version of Rekit Studio: 2.2.2

## How to use


```sh
# create project
docker run -v $(pwd):/home/node/app dimasmith/rekit rekit create <project>

# go to project directory
cd <project>

# install dependencies
docker run -v $(pwd):/home/node/app dimasmith/rekit yarn

# start project
docker run -v $(pwd):/home/node/app -p 6075:6075 -p 6076:6076 dimasmith/rekit yarn start
```

Open http://localhost:6076

Enjoy!
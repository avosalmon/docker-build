## Features
- Node
- Npm or Yarn
- Ionic
- Cordova

## Usage
```
docker run -it --rm -p 8100:8100 -p 35729:35729 -v /path/to/your/ionic-project/:/var/app/current avosalmon/ionic
```

## Alias
```
alias ionic="docker pull avosalmon/ionic:latest && docker run -it --rm --net host --privileged -v \$PWD:/var/app/current avosalmon/ionic"
```
> Due to a bug in ionic, if you want to use ionic serve, you have to use --net host option 

#### Example
```bash
ionic start myApp tabs
cd myApp
ionic serve
```

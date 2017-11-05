## Features
- Node
- Npm or Yarn
- Ionic
- Cordova

## Usage
```
docker run -it --rm -p 8100:8100 -p 35729:35729 -v /path/to/your/ionic-project/:/var/app/current avosalmon/ionic ionic
```

## Alias
```
alias ionic="docker run -it --rm -p 8100:8100 -p 35729:35729 -v \$PWD:/var/app/current -v ~/.gitconfig:/root/.gitconfig -v ~/.ssh:/root/.ssh avosalmon/ionic ionic"
alias ionic-push="docker run -it --rm -v \$PWD:/var/app/current -v ~/.gitconfig:/root/.gitconfig -v ~/.ssh:/root/.ssh avosalmon/ionic git push ionic master"
```
> Due to a bug in ionic, if you want to use ionic serve, you have to use --net host option 

#### Example
```bash
ionic start myApp tabs
cd myApp
ionic serve
```

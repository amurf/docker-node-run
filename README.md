# docker-node-run

CLI to run node projects in a docker container. 

## Useful

Add this to your `.bashrc` file: 

`alias node-run='docker run -it --rm -p 8080:8080 -v "$PWD:/node-run" amurf/node-run'`

note: you may need to update the default port mapping

## Examples

Running a simple express app

```
cd node-express-application
node-run node server.js
```

or

Running npm commands

```
cd vuejs-app/
node-run npm run dev
```

or 

Running webpack

```
cd webpack-app/
node-run webpack
```

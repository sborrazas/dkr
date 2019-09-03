# dkr

Docker environment virtualization tool.

## Usage

```
$ cat .dkr
IMAGE=node:8.16.1
DKR_OPTS="--network=mynet"
```

You can now run commands using the Docker image inside the project directory.

```
$ dkr npm start
```

Alternatively, you can use it without the `.dkr` file, using environment variables instead:

```
$ IMAGE=node:8.16.1 dkr npm start
```

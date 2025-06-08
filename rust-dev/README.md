# C, C++ development image

## Environment variables

To preserve user permissions on file a new user is created inside the container to match the user id and group id.
If your user has different values than `1000:1000` then add `UID` and `GID` environment variables.

```BASH
UID=$(id -u)
GID=$(id -g)
```

## Working directory inside container

Mount volumes inside this directory to match files permissions.

`/home/user/app`

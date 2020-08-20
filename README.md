# dockertest.sh

## What dockertest do
This is an utility script that allow you to quickly test a dockerfile. It firstly build and run the dockerfile, if you launch it again it kill the old docker and build and run the newer.  

## Download repository
```git clone https://github.com/ZappaBoy/dockertest.sh.git```

## Add the script to `/usr/bin/`
```
cd dockertest.sh/
cp dockertest /usr/bin/ 
```
## Usage
dockertest **DOCKER_TAG** **DOCKERFILE_PATH** **OTHER_DOCKER_PARAMETERS**

## Other docker parameters
You can add all docker parameters accepted by docker ad `-d ` parameter
### Example
```
dockertest testing_tag . -d --restart=always
```

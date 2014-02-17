## jpaas-buildpack-golang

Buildpack for [Golang][go] based on [Heroku Buildpack][heroku-buildpack].

* .godir - contains the desired name of the final binary.
* Procfile - specifies the type of the application and the actual command executed when the instance is started.

## Example

    git clone https://github.com/jpaas-lib/jpaas-app-demos

    cd golang/
    appname="my-go-demo" # change to your own name

    jpaas push ${appname} -i 1 -m 64M -b https://github.com/jpaas-lib/jpaas-buildpack-golang
    curl ${appname}.jpaas-edu.baidu.com



[go]: http://golang.org/
[heroku-buildpack]: https://github.com/kr/heroku-buildpack-go.git

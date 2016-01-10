# Ruby on Rails Tutorial: "hello, world!"

This is the first application for the
[*Ruby on Rails Tutorial*](http://www.railstutorial.org/)


##Buildpack 

```shell 
cd <your app dir>
bundle package --all
```

```shell
cf push (using manifest.yml)
or
cf push bp_ror_hello_app -b https://github.com/cloudfoundry/ruby-buildpack.git  -m 512MB -c "bundle exec rails s -b 0.0.0.0 -p 8080" 
````

##Docker 


```shell
cf push docker_ror_hello_app --docker-image <dockerimage>  -m 512MB -c "bundle exec rails se" 
````
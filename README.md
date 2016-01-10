# Ruby on Rails Tutorial: "hello, world!"

This is the first application for the
[*Ruby on Rails Tutorial*](http://www.railstutorial.org/)


* Buildpack push app
	cd <your app dir>
	bundle package --all

cf push (using manifest.yml)
or
cf push wy_ror_hello_app -b https://github.com/cloudfoundry/ruby-buildpack.git  -m 512MB -c "bundle exec rails s -b 0.0.0.0 -p 8080" 
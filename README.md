# Django API Table Of Content

- [Django API Table Of Content](#django-api-table-of-content)
  - [Setup](#setup)
  - [Questions](#questions)
  - [Links](#links)

## [Setup](#django-api-table-of-content)

~~using python 3.7: django-api-p37~~
installed docker for mac from: <https://hub.docker.com/editions/community/docker-ce-desktop-mac>
  => folowed regular mac installation of any .dmg file and once isntalled, started the application  
crated a Diockerfile, to learn more check it out  
when creating requirement.txt for django version and djangorestframeowrk i searched:  
  <https://pypi.org/project/Django/>  

`Dockerfile build .` => build the image  
`docker-compose build` => build a service on the image  
  run this again, if adding new pacakged to requirement.txt  
`docker-compose run app sh -c "django-admin.py startproject app ."` build django service on our image  
`docker-compose run app sh -c "python manage.py test"` run my unit tests  
`docker-compose run app sh -c "python manage.py test and flake8"` run my unit tests with linting
`docker-compose run app sh -c "python manage.py startapp core"` creating a new plugin (forgot best term)  
  per video, where my core code lives.  
  we deleted the view.py and tests.py => just play along :-)  
`docker-compose run app sh -c "python manage.py makemigrations core"` => updating db 


## [Questions](#django-api-table-of-content)

Dockerfile VS Compose  
  <https://stackoverflow.com/questions/29480099/docker-compose-vs-dockerfile-which-is-better>  
  <https://www.hostinger.com/tutorials/docker-start-a-container/>  

How can i access my dependencies/packaged when working project in on a docker container?  
  this is an issue since i cannot access my packages and see Class implementation when using inheritance  
  also when for instance overriding cache from from perm to temp 301 redirection, in this case i cannot until  
    having access to thos conda installed packages/ in this case is pip env - did not use conda for this project  
  `docker-compose run --rm --service-ports web bash` => to get to command line for the container  
  `docker exec -it <container ID> pip list` => execute command on container  
  `docker images` => this is how i can get container id  
  `docker exec -it <mycontainer> /bin/bash` => this is may be the way to accees container  
  `docker exec -it <mycontainer> sh` => this is may be the way to accees container  
Maybe i should use github action instead of Travis_CI since not free for private repos?  
Is flake8 the best liniting tool? Do a a bit of search and compare alternative.  

## [Links](#django-api-table-of-content)

 <https://www.django-rest-framework.org>  
<https://www.django-rest-framework.org/api-guide/views/>  
<https://docs.djangoproject.com/en/2.2/topics/testing/tools/#overview-and-a-quick-example> => links for Client documention
<>
<>
<>
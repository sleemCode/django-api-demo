# Django API Table Of Content

- [Django API Table Of Content](#django-api-table-of-content)
  - [Setup](#setup)
  - [Questions](#questions)
  - [Links](#links)

## [Setup](#django-api-table-of-content)

using python 3.7: django-api-p37           /Users/rajasleem/.conda/envs/django-api-p37
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
`docker-compose run app sh -c "python manage.py startapp core"` creating a new plugin (forgot best term)
  per video, where my core code lives.



## [Questions](#django-api-table-of-content)

Maybe i should use github action instead of Travis_CI since not free for private repos?
Is flake8 the best liniting tool? Do a a bit of search and compare alternative.

## [Links](#django-api-table-of-content)

<https://www.django-rest-framework.org>
<https://www.django-rest-framework.org/api-guide/views/>
<>
<>
<>
<>
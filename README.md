Django Nginx Jumpstart
======================

This repo contains a template for quickly setting up a Django/Nginx/Postgres/Supervisor environment on OSX. Inspired by https://github.com/oleksandr/django-buildout-layout.

Prerequisites
=============

* A Postgres DB with proper permssions

Get Started
===========

* Duplicate this repo:
```
git clone --bare git@github.com:jfberma/django-nginx-jumpstart.git
cd django-nginx-jumpstart.git
git push --mirror [YOUR_NEW_REPO_URL]
```

* clone your new repo
* ```cd``` into the new repo and edit ```buildout.cfg``` to include your enviroment's database details
* run ```scripts\devUpdate.sh```

That's it! You should not be able access your django site here: http://localhost:8080. Or https://localhost:8443 for SSL.

Recommendations
===============

* If you're using this template for multiple enivroments, after you mirror the repo, add buildout.cfg to .gitignore
* If you run into a bootstrap replated version error at the end of install, try running ```python bootstrap.py -v 2.1.1```


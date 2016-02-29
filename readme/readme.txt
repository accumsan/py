https://devcenter.heroku.com/articles/python-websockets
http://wallfloweropen.com/?project=heroku-app-for-convex-optimization
https://devcenter.heroku.com/articles/buildpacks

git clone git@github.com:heroku-examples/python-websockets-chat.git
-------on local---------
pip install Flask Flask-Sockets Gunicorn redis
export REDIS_URL='redis://localhost:6379'
heroku local
-------deploy-----------
heroku create minhdd-py --buildpack https://github.com/kennethreitz/conda-buildpack.git
heroku addons:create heroku-redis
git push heroku master

add conda-requirements and push
-------------------------------
scipy
numpy
scikit-learn
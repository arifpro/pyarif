# pyarif

- file -> save workspace as
- `pip install pipenv`
- install jupyter: `pipenv install jupyter --python 3.8`
- to activate virtual environment: `pipenv shell`
- run notebook: `jupyter notebook`
- create hash pass: `ipython -c "from notebook.auth import passwd; passwd()"`
- or, `python -c "from notebook.auth import passwd; print(passwd())"`
- run notebook with pass: `jupyter notebook --config=./config/jupyter.py`
- `jupyter notebook --generate-config`
- `!tar chvfz notebook.tar.gz *`
- `!tar -xv -f notebook.tar.gz`
- `chmod +x scripts/entrypoint.sh`


## Build & Run Docker Locally

- build docker: `docker build -t pyarif -f Dockerfile .`
- docker run -it pyarif /bin/bash
- docker run --env PORT=8888 -it -p 8888:8888 pyarif


## chmod

- chmod +x ./scripts/d_build.sh
- chmod +x ./scripts/d_run.sh
- chmod +x ./scripts/d_buildAndRun.sh

## heroku

- Create heroku app: `heroku create pyarif`
- Login to Heroku Container Registry: `heroku container:login`
- Push To Heroku: `heroku container:push web`
- Release To Heroku: `heroku container:release web`

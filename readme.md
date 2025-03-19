
[![Continuus Integration](https://github.com/kb1907/GithubActions-DockerHub-CICD-Tutorial/actions/workflows/github-docker-cicd.yaml/badge.svg)](https://github.com/kb1907/GithubActions-DockerHub-CICD-Tutorial/actions/workflows/github-docker-cicd.yaml)

# Create an MLOps Pipeline With GitHub and Docker Hub in Minutes

- This repo contains application files for [Create an MLOps Pipeline With GitHub and Docker Hub in Minutes](https://heartbeat.comet.ml/create-an-mlops-pipeline-with-github-and-docker-hub-in-minutes-4a1515b6a551) article.

![dock](https://user-images.githubusercontent.com/51021282/193422115-788fdb65-8861-4206-bd23-8d387a216ae2.png).


```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python app.py
docker build -t mlops .
docker run -it --rm mlops / docker run -it -p 8080:5000 mlops 
docker login 
docker image tag mlops:latest cramdani/mlops-test:latest
docker push cramdani/mlops:latest
# docker compose up 
docker container ls # list container 
docker container commit ..    
```


```bash
git remote remove origin 
git remote add origin https://github.com/Cyren4/mlops_cours.git
git remote -v
git push --set-upstream origin main
```

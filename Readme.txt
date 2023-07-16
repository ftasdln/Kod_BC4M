git init
git status
git add .
git commit
git remote add
git clone "url"
vi Dockerfile
FROM python
COPY . /apps
WORKDIR /apps
RUN pip install -r requirements.txt
ENTRYPOINT python app.py
docker build --tag task
docker run --rm -i -t task
docker run --rm -i -t -p 8080:5000 task



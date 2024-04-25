
```dockerfile
FROM python:3.9-slim

WORKDIR /notebooks

RUN pip install --no-cache-dir notebook

VOLUME /notebooks

CMD ["jupyter", "notebook", "--ip='0.0.0.0'", "--port=8888", "--no-browser", "--allow-root", "--NotebookApp.token=''", "--NotebookApp.password=''", "--NotebookApp.notebook_dir=/notebooks"]
```

```shell
mkdir ~/notebooks
docker build -t my-python-jupyter .
docker run -p 80:8888 -v /notebooks:/notebooks my-python-jupyter

```

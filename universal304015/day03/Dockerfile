# 파이썬 베이스 이미지 사용
FROM python:3.9-slim

# 작업 디렉토리 설정
WORKDIR /notebooks

# 필요한 패키지와 Jupyter 설치
RUN pip install --no-cache-dir notebook

# 외부에 노트북 디렉토리 노출
VOLUME /notebooks

# Jupyter Notebook 실행 명령
CMD ["jupyter", "notebook", "--ip='0.0.0.0'", "--port=8888", "--no-browser", "--allow-root", "--NotebookApp.token=''", "--NotebookApp.password=''", "--NotebookApp.notebook_dir=/notebooks"]

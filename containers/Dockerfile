FROM python:latest

WORKDIR /work

COPY ./requirements.txt .

RUN pip install --upgrade pip
RUN pip install -r requirements.txt
RUN jupyter contrib nbextension install --user
RUN jupyter nbextensions_configurator enable --user

CMD ["jupyter", "lab", "--ip=0.0.0.0", "--allow-root", "--LabApp.token=''"]

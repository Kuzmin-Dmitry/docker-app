FROM centos:latest
MAINTAINER Dmitry Kuzmin 'kuzmin.mail@gmail.com'
RUN yum --enablerepo=extras install -y epel-release
RUN yum update -y
RUN yum install -y python-pip python-dev build-essential
RUN pip install --upgrade pip
COPY . /app
WORKDIR /app
RUN pip install -r requirements.txt
ENTRYPOINT ["python"]
CMD ["app.py"]

FROM python:3
RUN apt-get update \
	&& apt-get install -y --no-install-recommends \
		postgresql-client \
	&& rm -rf /var/lib/apt/lists/*
RUN mkdir diango_app
WORKDIR /diango_app
COPY requirements.txt /diango_app
RUN pip install -r requirements.txt
COPY . /diango_app
RUN touch /root/abdo77


EXPOSE 8000


#FROM python:3  as production
#RUN apt-get update \
#	&& apt-get install -y --no-install-recommends \
#		postgresql-client \
#	&& rm -rf /var/lib/apt/lists/*

#RUN mkdir diango_app
#WORKDIR /diango_app

#COPY requirements.txt /diango_app
#RUN pip install -r requirements.txt
#COPY . /diango_app
#EXPOSE 8000

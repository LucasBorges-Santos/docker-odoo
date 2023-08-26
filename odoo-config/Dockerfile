FROM ubuntu
FROM python:3.7

RUN pip install --upgrade pip && apt-get update
RUN apt-get install -y --no-install-recommends \
            ca-certificates \
            curl \
            dirmngr \
            fonts-noto-cjk \
            gnupg \
            libssl-dev \
            node-less \
            npm \
            python3-num2words \
            python3-pip \
            python3-phonenumbers \
            python3-pyldap \
            python3-qrcode \
            python3-renderpm \
            python3-setuptools \
            python3-slugify \
            python3-vobject \
            python3-watchdog \
            python3-xlrd \
            python3-xlwt \
            xz-utils \
            libsasl2-dev \
            libldap2-dev \
            libssl-dev

COPY odoo-files /opt

RUN pip install -r opt/odoo/requirements.txt

EXPOSE 8069
FROM quay.io/akretion/odoo:10.0-latest

COPY . /opt/odoo
COPY ./etc/odoo.cfg.tmpl /opt/etc/odoo.cfg.tmpl

RUN pip install -r /opt/odoo/requirements.txt
RUN pip install -e /opt/odoo
RUN pip install -e /opt/odoo/src

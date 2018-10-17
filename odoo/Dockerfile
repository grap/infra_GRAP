# FROM camptocamp/odoo-project:12.0-latest-batteries
# Commented, when docky run, the following error occures.
#/odoo/src/odoo.egg-info is missing, probably because the directory is a volume.
#Running pip install -e /odoo/src to restore odoo.egg-info
#/odoo/src should either be a path to a local project or a VCS url beginning with svn+, git+, hg+, or bzr+

FROM quay.io/akretion/odoo:11.0-full-latest

COPY . /opt/odoo
COPY ./etc/odoo.cfg.tmpl /opt/etc/odoo.cfg.tmpl

RUN pip install -r /opt/odoo/requirements.txt
RUN pip install -e /opt/odoo
RUN pip install -e /opt/odoo/src

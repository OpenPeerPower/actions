FROM openpeerpower/open-peer-power:beta

COPY entrypoint.sh /entrypoint.sh
COPY requirements.txt .

RUN pip3 install -r requirements.txt

WORKDIR "/github/workspace"
ENTRYPOINT ["/entrypoint.sh"]

LABEL "name"="oppfest"
LABEL "maintainer"="Open Peer Power <hello@open-peer-power.io>"
LABEL "version"="1.1"

LABEL "com.github.actions.name"="oppfest"
LABEL "com.github.actions.description"="Run oppfest to validate standalone integration repositories"
LABEL "com.github.actions.icon"="terminal"
LABEL "com.github.actions.color"="gray-dark"

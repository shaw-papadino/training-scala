# [Choice] Java version: 11, 15
ARG VARIANT=$VARIANT
FROM mcr.microsoft.com/vscode/devcontainers/java:${VARIANT}

# [Option] Install sbt
ARG INSTALL_SBT="true"
RUN if [ "${INSTALL_SBT}" = "true" ]; then \
    echo "deb https://repo.scala-sbt.org/scalasbt/debian all main" > /etc/apt/sources.list.d/sbt.list \
    && echo "deb https://repo.scala-sbt.org/scalasbt/debian /" > /etc/apt/sources.list.d/sbt_old.list \
    && curl -sL "https://keyserver.ubuntu.com/pks/lookup?op=get&search=0x2EE0EA64E40A89B84B2DF73499E82A75642AC823" | apt-key add \
    && apt-get update \
    && apt-get install sbt \
    && apt-get clean -y && rm -rf /var/lib/apt/lists/* ; fi

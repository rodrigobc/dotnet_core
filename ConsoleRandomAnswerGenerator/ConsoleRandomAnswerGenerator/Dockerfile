FROM sixeyed/coreclr-base:1.0.0-rc1-final

# ensure the expected DNX is available
ENV PATH /root/.dnx/runtimes/dnx-coreclr-linux-x64.1.0.0-rc1-final/bin:$PATH

# deploy the  app
COPY /. /opt/consolerandomanswergenerator
WORKDIR opt/consolerandomanswergenerator
RUN dnu restore

ENTRYPOINT ["dnx", "run"]

FROM microsoft/dotnet-nightly
WORKDIR /app
ENV ASPNETCORE_URLS http://+:80
EXPOSE 80
COPY . /app
RUN dotnet restore
ENTRYPOINT ["dotnet","run"]

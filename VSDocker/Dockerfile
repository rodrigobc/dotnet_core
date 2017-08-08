#FROM microsoft/dotnet-nightly
FROM microsoft/dotnet:1.0-sdk-projectjson
WORKDIR /app
ENV ASPNETCORE_URLS http://+:80
EXPOSE 80
COPY . /app
RUN dotnet restore
ENTRYPOINT ["dotnet","run"]

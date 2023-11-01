FROM mcr.microsoft.com/dotnet/sdk:7.0 AS build-env
WORKDIR /worker
COPY . ./
RUN dotnet restore

RUN dotnet publish -c Release -o out
FROM mcr.microsoft.com/dotnet/aspnet:7.0
WORKDIR /worker
COPY --from=build-env /worker/out .
ENTRYPOINT ["dotnet", "DotNet.Docker.dll"]
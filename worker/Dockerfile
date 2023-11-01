FROM mcr.microsoft.com/dotnet/sdk:7.0-alpine
WORKDIR /worker
COPY . .
RUN ["dotnet", "restore"]
RUN ["dotnet", "publish", "-c", "release", "--self-contained", "false", "--no-restore"]
CMD ["dotnet", "bin/release/net7.0/Worker.dll"]
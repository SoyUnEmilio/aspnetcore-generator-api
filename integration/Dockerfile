#build stage
FROM microsoft/dotnet:2.0.0-sdk

WORKDIR /integration

# restore
COPY integration.csproj .
RUN dotnet restore

# copy src
COPY .  .

ENTRYPOINT [ "dotnet", "test" ]
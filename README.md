# aspire-dashboard-sidecar-java
example of running the .net aspire dashboard as a sidecar when using devcontainers for a java application

# links

- [Standalone .NET Aspire Dashboard](https://learn.microsoft.com/en-us/dotnet/aspire/fundamentals/dashboard/standalone?tabs=bash)

# notes

docker run --rm -it -p 18888:18888 -p 4317:18889 -d --name aspire-dashboard mcr.microsoft.com/dotnet/aspire-dashboard:9.0 \
    -e DOTNET_DASHBOARD_UNSECURED_ALLOW_ANONYMOUS='true' \
    -e Dashboard__Frontend__AuthMode='Unsecured'

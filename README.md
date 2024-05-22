# RenGzWeb
A from scratch rewrite of Gazebo Web Server

## Options

- We want modern support for gRPC as Gazebo uses gRPC, and we think that it could be easier to port some of the mechanisms more
directly.

- On the front-end we want to support something like React/Next.js/threejs to display 3d objects.

Few options we came across:

1. grpc-web: https://github.com/grpc/grpc-web
- quite basic, and may need to implement other functionality for a full web server

2. gunicorn

3. grpcWSGI https://pypi.org/project/grpcWSGI/

4. ASP .NET over nginx

https://learn.microsoft.com/en-us/aspnet/core/host-and-deploy/linux-nginx?view=aspnetcore-8.0&tabs=linux-ubuntu

https://github.com/grpc/grpc-dotnet/issues/1905

https://github.com/grpc/grpc-dotnet/

2024-May-22: we decided to try out ASP .NET over nginx and build a server layer around gazebo headless server.
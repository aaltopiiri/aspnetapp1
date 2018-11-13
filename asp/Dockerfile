FROM microsoft/aspnetcore-build:lts
COPY ./app /app
WORKDIR /app
RUN ["dotnet", "restore"]
RUN ["dotnet", "build"]
ENV ASPNETCORE_URLS http://+:5000
EXPOSE 5000
RUN chmod +x ./entrypoint.sh
CMD /bin/bash ./entrypoint.sh
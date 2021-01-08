# android-teamcity-buildagent

Dockerfile для создания образа Teamcity buildagent, который сможет собирать Android проекты

Создан на основе https://hub.docker.com/r/azabost/android-sdk-teamcity-agent/dockerfile

```
docker run -it -e SERVER_URL="<url to TeamCity server>"  \ 
    -v <path to agent config folder>:/data/teamcity_agent/conf  \      
    jetbrains/teamcity-agent
```

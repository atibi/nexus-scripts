Sonatype Nexus REST and Integration API scripts
===============================================

Scripts for REST and Integration API as documented in http://books.sonatype.com/nexus-book/reference3/scripting.html

findByGroupIdAndExtension:: JSON script that list artifacts of a maven2 repository

```
curl -v -X POST -u admin:admin123 --header "Content-Type: text/plain" "http://localhost:8081/service/siesta/rest/v1/script/findByGroupIdAndExtension/run" -d '{"repoName":"maven-releases","groupId":"com.mondora", "extension":"jar"}'
```
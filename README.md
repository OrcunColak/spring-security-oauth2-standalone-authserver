# Read me
This Authentication Server is for client_credentials

The original idea is from  
https://neuw.medium.com/spring-boot-3-oauth2-client-for-servlets-based-project-1343de8bab34

Git  
https://github.com/krnbr/spring-oauth2-server/tree/main

1. Send POST request to Authentication Server http://localhost:64200/oauth2/token and get token
2. Send GET request to Resource Server  http://localhost:64203/test with token
3. Resource server contacts Authentication Server http://localhost:64200/oauth2/introspect
4. Resource server send Http 200 
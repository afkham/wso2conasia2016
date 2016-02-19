## Demonstrates how to secure microservices using OAuth2

This step requires running WSO2 Identity Server (IS). For more details, see [https://github.com/wso2/msf4j/tree/master/samples/security](https://github.com/wso2/msf4j/tree/master/samples/security)

Commands
--------

1.
curl -v http://localhost:8080/stockquote/IBM

2.
curl -v -k -X POST --basic -u bXlSnEjTJYK9wSmAaLk5JFIHy3ka:qIvB8p2PFaKt7bn6QeKSnaJK80Ma  -H "Content-Type: application/x-www-form-urlencoded;charset=UTF-8" -d "grant_type=client_credentials" https://localhost:9443/oauth2/token

See: [https://github.com/wso2/msf4j/tree/master/samples/security](https://github.com/wso2/msf4j/tree/master/samples/security) 

3.
curl -v -H "Authorization: Bearer 98dc95e8c067848017573d44c20189fe" http://localhost:8080/stockquote/IBM


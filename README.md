# soap-ws
>About the generated source found in client/src/main/java/soap/ws/server and shared package, they're generated by the following steps

```
#used to get the wsdl file of the service and put in the selected package
cd client/src/main/java
curl "http://127.0.0.1:9090/Hello?wsdl" --output service.wsdl

#used to generate the sources not compiled by the wsdl file
wsimport service.wsdl -Xnocompile
```

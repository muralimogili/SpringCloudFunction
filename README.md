# Spring Cloud Function example

## Exposed Functions as Endpoints
- *Supplier* - `/supply` - returns an output

```
curl -H 'Content-Type: text/plain' http://localhost:8080/supply
Hello Youtube⏎                                                                                                      

```

- *Consumer* - `/consume` - expects an input

```
curl -H 'Content-Type: text/plain' http://localhost:8080/consume -d 'Hello Veeraswamy'
```

- *Function* - `/function` - expects an input and output
```
curl -H 'Content-Type: text/plain' http://localhost:8080/function -d 'Hello Veeraswamy'
Hello Veeraswamy⏎    
```

- *Function* - `/hello` - expects an input and output
```                                                                                        
curl -H 'Content-Type: text/plain' http://localhost:8080/hello -d 'Veeraswamys'
Hello Veeraswamys⏎  
```
### install

```bash
go get github.com/cntech-io/cntechkit-redis/v2
```

## Methods

| Method                                                                  | Description                                                     |
| ----------------------------------------------------------------------- | --------------------------------------------------------------- |
| request.NewCollection(collectionName string, options CollectionOptions) | Creates collection instance                                     |
| &nbsp;&nbsp;&nbsp;&nbsp;.AddRequest(r Request)                          | Adds request to collection                                      |
| &nbsp;&nbsp;&nbsp;&nbsp;.Log()                                          | Shows collection data                                           |
| &nbsp;&nbsp;&nbsp;&nbsp;.CreateClients()                                | Creates clients ready to make http request                      |
| "clientVariable".Result(key string)                                     | Makes http request to collection request with corresponding key |
| request.NewGetRequest(key string, url string)                           | Creates GET request                                             |
| request.NewPostRequest(key string, url string)                          | Creates POST request                                            |
| request.NewPatchRequest(key string, url string)                         | Creates PATCH request                                           |
| request.NewPutRequest(key string, url string)                           | Creates PUT request                                             |
| request.NewDeleteRequest(key string, url string)                        | Creates DELETE request                                          |
| &nbsp;&nbsp;&nbsp;&nbsp;.AddHeader(key string, value string)            | Adds header to request                                          |
| &nbsp;&nbsp;&nbsp;&nbsp;.AddBearerHeader(token string)                  | Adds Bearer header to request                                   |
| &nbsp;&nbsp;&nbsp;&nbsp;.AddContentTypeJsonHeader()                     | Adds "content-type":"application/json" header to request        |
| &nbsp;&nbsp;&nbsp;&nbsp;.AddQuery(key string, value string)             | Adds query to request                                           |
| &nbsp;&nbsp;&nbsp;&nbsp;.AddPath(path string)                           | Adds path to request                                            |
| &nbsp;&nbsp;&nbsp;&nbsp;.AddBody(body interface{})                      | Adds body to request                                            |
| &nbsp;&nbsp;&nbsp;&nbsp;.AddBasicAuth(username string, password string) | Adds basic auth to request                                      |

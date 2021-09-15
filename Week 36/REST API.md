# Rest API

## Creat a rest api

```mermaid
flowchart TD

 subgraph BackendTier
    subgraph UI
    Console.App
    web.api
    end
    subgraph Infrastructure
    DataSql
    dataInMemory
    end
    subgraph Domain
    core
    domain
    end

    web.api --> domain
end
    subgraph FrontendTier
    Angular
    Mobile

    end
 Angular --who is sending where is it going budy text 'json' get, post, put, delete, patch--> www
 www --trans HTTP to C# --> web.api
 
 Domain --- Infrastructure
 web.api-->www
 www-->Angular
 
 PostMan
```

- Read - Get(no text body : always only read data , not to send data.)
- Update - Put - patch(part of update)



## Json

- Make the object as string in an array

```json
[{
    "data":00,"name":fei
}]
```



## Test it by PostMan

## CRUD





# 

# HTML traffic flow

```plantuml
left to right direction

actor "User web browser" as user
cloud "Auth server" as [auth-server]

user --> [Ui]
user --> [Gateway.Api]

[Gateway.Api] -left-> [auth-server]
[Gateway.Api] --> [News.Api]
[Gateway.Api] --> [Products.Api]
[Gateway.Api] --> [Documents.Api]
[Gateway.Api] --> [Content.Api]
```

## H2 Connection

h2  설정 후 console에서 접속시 아래 에러메시지가 나타나는 경우 
```
spring boot either pre-create it or allow remote database creation (not recommended in secure environments) [90149-200] 90149/90149 (help)
```

터미널에서 h2 설치 후 접속
```
$ brew install h2
$ h2 -web
Web Console server running at http://localhost:8082?key=e5e8e93d1eb5e1ffce5fdfd1967f450b8c958857f5d67e996ad25f48ad6d9547 (only local connections)
```
아래 설정처럼 변경하고 접속 > 터미널의 h2종료 > spring boot console 접속  
>Saved Settings : Generic H2(server) 
>JDBC URL : 'spring boot console과 동일하게 설정'  


-----

## command
```s
docker build -t docker-unoconv-webservice .
docker run -d -p 4000:3000 --name unoconv docker-unoconv-webservice
curl --form "file=@/Users/keeley/Downloads/决策树算法.ppt" http://localhost:4000/unoconv/pdf > "决策树算法.ppt.pdf"
```

貌似只能玩玩，线上文档多了扛不住，web没挂但是里面的office.bin容易假死。。已经没用这个了。

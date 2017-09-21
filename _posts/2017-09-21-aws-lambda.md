---
layout: post
title: 'AWS Lambda DynamoDB API Gateway 연동기'
author: dskim
date: 2017-09-21 18:09
tags: [aws]
image: /files/covers/aws-lambda-apigate-dynamodb.jpg
---

## NOSQL로 데이터를 쌓아야하는 행위가 필요했다.

위치정보를 쌓아야하는 미션이다. 하지만 일단 로우데이터라 

일단 쌓아야 하므로.. AWS DynamoDB와 AWS의 API Gateway와 Lambda를 이용해서 

일단 이렇게 만들생각을하고 일단 -ㅅ-...실행


<img src="/files/2017-09-21-aws-lambda-1.png" class="hcenter">

## AWS Services -> DynamoDB 테이블 만들기

<img src="/files/2017-09-21-aws-lambda-2.png" class="hcenter">



## AWS Services 테이블설계

<img src="/files/2017-09-21-aws-lambda-3.png" class="hcenter">
nosql방식이라 일단 정렬키는 잘몰라서 기본키베이스로 설계를 했다.
```
{
    "UID" : "",
    "ZID" ; "",
    "PARTNER_ID" : "",
    "LONGTITUDE" : "",
    "LATITUDE" : "",
    "ESTIMATE_NO" : "",
    "CREATE_DATE" : ""
}

```


### AWS Lambda 함수 생성


<img src="/files/2017-09-21-aws-lambda-3.png" class="hcenter">
추후 정리해서 다시 적어야겠다;
# Serverless Practice 1
DynamoDB, Lambda, API Gateway 를 이용해 AWS 데이타베이스와 통신하는 방법의 기초 <br>

## Serverless Access key, Secret Key 세팅방법
[Serverless Reference](https://www.serverless.com/framework/docs/providers/aws/guide/credentials/)

## Serverless 에러들과 헤걀방법
[Link](https://www.stackery.io/blog/top-10-deployment-errors/)

## 중복되는 Resource
에러 메세지: <br>
```
An error occurred: NotesTable - sls-practice-note-backend-prod already exists in stack arn:aws:cloudformation:us-west-2:504507559414:stack/sls-practice-note-backend-prod/19ab5290-453a-11eb-8c38-0605a89bca9d.
```

이렇게 `already exists in stack` 에러가 나오면 <br>
[여기 참조](https://aws.amazon.com/ko/premiumsupport/knowledge-center/cloudformation-stack-resource-failure/)

내 경우에는 `DeletionPolicy` 가 문제가 되는것 같았다. 

## 테스트 방법 


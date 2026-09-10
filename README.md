# Interview даалгавар: Serverless Notification Request System

## Тойм

Notification request удирдах жижиг full-stack serverless application бүтээнэ.

Систем нь frontend application-оос хэрэглэгч notification request үүсгэх боломжтой байна. Backend нь тухайн request-ийг хүлээн авч, хадгалж, asynchronous processing хийхэд бэлдэнэ.

Энэ даалгавар нь зориуд нээлттэй байдлаар өгөгдсөн. Та өөрөө боломжийн technical decision-үүд гаргаж, тэдгээрийг README дээрээ тайлбарлана.

## Хугацаа

Энэ даалгаврыг гүйцэтгэх хугацаа **3 өдөр**.

Clean, correct, maintainable solution гаргахад төвлөрнө. Хэт over-engineer хийх шаардлагагүй.

## Ашиглах шаардлагатай tech stack

### Backend

- TypeScript
- Node.js
- Serverless Framework
- AWS Lambda
- API Gateway
- DynamoDB
- SQS

### Frontend

Дараахын аль нэгийг ашиглана:

- React
- Next.js
- Vite + React

Frontend дээр TypeScript ашиглах шаардлагатай.

## Даалгавар

Serverless notification request system бүтээнэ.

Application дараах ерөнхий behavior-ийг дэмждэг байна:

1. Хэрэглэгч frontend-оос notification request submit хийх боломжтой байна.
2. Backend илгээгдсэн request-ийг хүлээн авч, validate хийх боломжтой байна.
3. Шаардлага хангасан notification request-үүд DynamoDB-д хадгалагдана.
4. Хадгалагдсан notification request-үүд тодорхой status эсвэл lifecycle-тэй байна.
5. Notification request-үүд SQS ашиглан asynchronous processing flow руу илгээгдэнэ.
6. Frontend илгээсэн notification request-үүд эсвэл submit хийсэн request-ийн result-ийг харуулах боломжтой байна.
7. Frontend амжилттай болон амжилтгүй action-д ойлгомжтой feedback харуулна.

## Та өөрөө шийдэх зүйлс

Та дараах зүйлсийг өөрөө шийднэ:

- Notification request-ийн data structure
- API endpoint design
- Request болон response format
- Validation strategy
- DynamoDB table design
- DynamoDB key structure
- SQS message structure
- Lambda function structure
- Нэг Lambda ашиглах уу эсвэл олон Lambda ашиглах уу
- Asynchronous processing flow хэрхэн ажиллах
- Frontend болон backend code-ийг хэрхэн зохион байгуулах
- Юуг test хийх шаардлагатай гэж үзэх
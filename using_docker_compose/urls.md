

curl -X GET --header 'Accept: application/json' --header 'Authorization: Bearer eyJhbGciOiJIUzUxMiJ9.eyJzdWIiOiJhZG1pbiIsImF1dGgiOiJST0xFX0FETUlOLFJPTEVfVVNFUiIsImV4cCI6MTU3NDI0NjgzMX0.HrE68KnbvcON0A5F7XJqR6vzOLYOh2LjzyzMGZHIWzDF0wJpcZO61n35z0aU5rwW_TpS7fJYDbx0lxMO9RTTCg' 'http://localhost:8080/services/invoice/api/invoices'


## Store API

### OrderItem Resource
#### GET

GET /api/order-items                                            getAllOrderItems
curl -X GET --header 'Accept: application/json' --header 'Authorization: Bearer eyJhbGciOiJIUzUxMiJ9.eyJzdWIiOiJhZG1pbiIsImF1dGgiOiJST0xFX0FETUlOLFJPTEVfVVNFUiIsImV4cCI6MTU3NDI0NjgzMX0.HrE68KnbvcON0A5F7XJqR6vzOLYOh2LjzyzMGZHIWzDF0wJpcZO61n35z0aU5rwW_TpS7fJYDbx0lxMO9RTTCg' 'http://localhost:8080/api/order-items'



POST /api/order-items                                             createOrderItem

curl -X POST --header 'Content-Type: application/json' --header 'Accept: application/problem+json' --header 'Authorization: Bearer eyJhbGciOiJIUzUxMiJ9.eyJzdWIiOiJhZG1pbiIsImF1dGgiOiJST0xFX0FETUlOLFJPTEVfVVNFUiIsImV4cCI6MTU3NDI0NjgzMX0.HrE68KnbvcON0A5F7XJqR6vzOLYOh2LjzyzMGZHIWzDF0wJpcZO61n35z0aU5rwW_TpS7fJYDbx0lxMO9RTTCg' -d '{ \ 
   "id": 0, \ 
   "order": { \ 
     "code": "string", \ 
     "customer": { \ 
       "addressLine1": "string", \ 
       "addressLine2": "string", \ 
       "city": "string", \ 
       "country": "string", \ 
       "email": "string", \ 
       "firstName": "string", \ 
       "gender": "MALE", \ 
       "id": 0, \ 
       "lastName": "string", \ 
       "orders": [ \ 
         {} \ 
       ], \ 
       "phone": "string", \ 
       "user": { \ 
         "activated": true, \ 
         "email": "string", \ 
         "firstName": "string", \ 
         "id": 0, \ 
         "imageUrl": "string", \ 
         "langKey": "string", \ 
         "lastName": "string", \ 
         "login": "string", \ 
         "resetDate": "2019-11-19T10:49:34.051Z" \ 
       } \ 
     }, \ 
     "id": 0, \ 
     "invoiceId": 0, \ 
     "orderItems": [ \ 
       {} \ 
     ], \ 
     "placedDate": "2019-11-19T10:49:34.052Z", \ 
     "status": "COMPLETED" \ 
   }, \ 
   "product": { \ 
     "description": "string", \ 
     "id": 0, \ 
     "name": "string", \ 
     "price": 0, \ 
     "productCategory": { \ 
       "description": "string", \ 
       "id": 0, \ 
       "name": "string", \ 
       "products": [ \ 
         {} \ 
       ] \ 
     }, \ 
     "size": "S" \ 
   }, \ 
   "quantity": 0, \ 
   "status": "AVAILABLE", \ 
   "totalPrice": 0 \ 
 }' 'http://localhost:8080/api/order-items'
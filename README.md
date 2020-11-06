# payment-orchestration-doc
API signatures for payment orchestration can be found here

## APIs

### PostAuth:

#### [initiatePostAuthPayment](apiReqRes/initiatePostAuthPayment) 
> Consumed by mobile app. Will return payment URL

#### [commitPostAuthPayment](apiReqRes/commitPostAuthPayment) 
> Consumed by ESB. Triggered when post auth payment is successful 

### PreAuth:

#### [reservePump](apiReqRes/reservePump) 
> Consumed by mobile app, initates preAuthFlow. Will return payment link

#### [activatePump](apiReqRes/activatePump) 
> Consumed by ESB, Triggered when pre auth payment is successful

#### [finalizeTransaction]() 
> Consumed by POS to send order details to orchestration

#### [commitPreAuthPayment](apiReqRes/commitPreAuthPayment) 
> Consumed by ESB. Triggered when pre auth payment is successful 

### Common API

#### [listPayments](apiReqRes/listPayments) 
> Consumed by mobile app, lists payment history for an user

_The api request/response shared here might get changed to accomodate any shortcomings_

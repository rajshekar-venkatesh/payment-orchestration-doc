# payment-orchestration-doc
API signatures for payment orchestration can be found here

## APIs

### PostAuth:

#### [initiatePostAuthPayment](apiReqRes/initiatePostAuthPayment) | [API Endpoint](https://wfq6iadb6k.execute-api.ap-southeast-1.amazonaws.com/default/initiatePostAuthPayment)
> Consumed by mobile app. Will return payment URL

#### [commitPostAuthPayment](apiReqRes/commitPostAuthPayment) | [API Endpoint](https://opzt9x8nni.execute-api.ap-southeast-1.amazonaws.com/default/commitPostAuthPayment)
> Consumed by ESB. Triggered when post auth payment is successful 

### PreAuth:

#### [reservePump](apiReqRes/reservePump) | [API Endpoint](https://lmotdgxhtl.execute-api.ap-southeast-1.amazonaws.com/default/reservePump)
> Consumed by mobile app, initates preAuthFlow. Will return payment link

#### [activatePump](apiReqRes/activatePump) | [API Endpoint](https://1oe4t902t4.execute-api.ap-southeast-1.amazonaws.com/default/activatePump) 
> Consumed by ESB, Triggered when pre auth payment is successful

#### [finalizeTransaction](apiReqRes/finalizeTransaction) | [API Endpoint](https://1oe4t902t4.execute-api.ap-southeast-1.amazonaws.com/default/finalizeTransaction) 
> Consumed by POS to send order details to orchestration

#### [commitPreAuthPayment](apiReqRes/commitPreAuthPayment) | [API Endpoint](https://1oe4t902t4.execute-api.ap-southeast-1.amazonaws.com/default/commitPreAuthPayment)  
> Consumed by ESB. Triggered when pre auth payment is successful 

### Common API

#### [listPayments](apiReqRes/listPayments) | [API Endpoint](https://1oe4t902t4.execute-api.ap-southeast-1.amazonaws.com/default/listPayments)  
> Consumed by mobile app, lists payment history for an user


* _The api request/response shared here might get changed to accomodate any shortcomings_

* _Authentication related info will be added soon_

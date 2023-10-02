## CostPay

Request

    type: CostPay
    access: (access token)
    vendor: (vendor id)

Response

    type: CostPay
    uri: (URI for the payment)

## CostGet

Request

    type: CostGet
    access: (access token)

Response

    type: CostGet
    credit: (i64 credit string)

The credit can be negative. `$CREDIT_LIMIT` sets the minimum.

## CostCheckIn

Request

    type: CostCheckIn
    access: (access token)

Response

    type: CostCheckIn
    award: (i64 award string)

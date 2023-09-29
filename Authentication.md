The http method is `POST` from now on, because only pinging doesn't change the server state.

## For testing servers with `SKIP_AUTH`

The `AuthSmsSent` request,

    type: AuthSmsSent
    access: (access token)
    refresh: (refresh token)
    phone: (phone number)
    message: (message token)

Authenticates the user as the owner of `phone number`.

## AuthSessionStart

Request

    type: AuthSessionStart

Response

    type: AuthSessionStart
    access: (access token)
    refresh: (refresh token)

## AuthSessionRefresh

Request

    type: AuthSessionRefresh
    refresh: (refresh token)

Response

    type: AuthSessionRefresh
    access: (new access token)

## AuthSessionEnd

Request

    type: AuthSessionEnd
    access: (access token)
    refresh: (refresh token)    <-- optional

Response

    type: AuthSessionEnd

## AuthSmsSendTo

Request

    type: AuthSmsSendTo
    access: (access token)

Response

    type: AuthSmsSendTo
    phone: (phone number)
    message: (message token)

Send SMS `message token` to `phone number` to verify phone number.

## AuthSmsSent

Request

    type: AuthSmsSent
    access: (access token)
    refresh: (refresh token)
    phone: (sent to phone number, not user phone number)
    message: (message token)

Response

    type: AuthSmsSent
    uid: (user id)

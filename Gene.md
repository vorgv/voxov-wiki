<type>

    type: (api name)

<head>

    access: (access token)
    time: (time cost)
    space: (space cost)
    traffic: (traffic cost)
    tip: (tip cost)
    fed: (optional fed id)

<changes>

    time: (time change)
    space: (space change)
    traffic: (traffic change)
    tip: (tip change)

## GeneMeta

Request

    <type>
    <head>
    gid: (gene's name)

Response

    <type>
    <changes>
    meta: (meta data in json)

## GeneCall

Request 

    <type>
    <head>
    gid: (gene's name)
    arg: (arguments)

Response

    <type>
    <changes>
    result: (output of the call)

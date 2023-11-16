<body>: http message body

## MemeMeta

Request

    <type>
    <head>
    hash: (blake3 hash of the meme)

Response

    <type>
    <changes>
    meta: (meme metadata in json)

## MemePut

Request

    <type>
    <head>
    days: (days to keep the meme)
    raw: <body> (raw bytes of the meme)

Response

    <type>
    <changes>
    hash: (blake3 hash of the meme)

## MemeGet

Request

    <type>
    <head>
    hash: (blake3 hash of the meme)
    public: true/false (search public memes?)

Response

    <type>
    <changes>
    raw: <body> (raw bytes of the meme)

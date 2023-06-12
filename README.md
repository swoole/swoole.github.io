```php
<?php

$server = new Swoole\Http\Server('0.0.0.0', 9501);

$server->on('start', function () {
    echo "Listening at http://localhost:9501\n";
});

$server->on('request', function ($req, $res) {
    $res->end('Hello, World!');
});

$server->start();
```

- [Swoole project](https://github.com/swoole)
- [Official website 🇨🇳](https://www.swoole.com)
- [Official wiki 🇨🇳](https://wiki.swoole.com)
- [**English community website, docs & blog**](https://swoole.dev)

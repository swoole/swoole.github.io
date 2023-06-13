<p class="lead my-5">
Open-Source High-Performance Application Server for PHP with Non-Blocking I/O & Asynchronous Coroutines. 
</p>

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

<ul class="nav mt-5">
	<li class="nav-item"><a class="btn btn-outline-primary" href="https://github.com/swoole"><i class="bi bi-github"/> Swoole project</a></li>
	<li class="nav-item"><a class="btn btn-outline-primary" href="https://www.swoole.com">🇨🇳 Official website</a></li>
	<li class="nav-item"><a class="btn btn-outline-primary" href="https://wiki.swoole.com">🇨🇳 Official wiki</a></li>
</ul>

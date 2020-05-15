# echo-boilerplate [![Go Report Card](https://goreportcard.com/badge/github.com/admiralobvious/echo-boilerplate)](https://goreportcard.com/report/github.com/admiralobvious/echo-boilerplate)

Boilerplate sederhana menggunakan framework minimalis [echo](https://github.com/labstack/echo)
dengan mengikuti [12-factor](https://12factor.net/) serta golang-standards' [project-layout](https://github.com/golang-standards/project-layout).

### Membangun dan menjalankan secara lokal
```shell script
go build ./cmd/app && ./app
```

### Menggunakan
```shell script
Penggunaan ./app:
      --app-name string               Nama aplikasi kamu. Digunakan untuk variabel prefix environment. (bawaan "app")
      --bind-address ip               IP yang akan dipantau. (bawaan 127.0.0.1)
      --bind-port uint                Port yang akan dipantau. (bawaan 1323)
      --cors-allow-credentials        Menyatakan kepada browser untuk mengungkap respon server ke bagian frontend Javascript ketika mode permintaan kredensial (Request.credentials) diserakan.
      --cors-allow-headers strings    Menyatakan HTTP header mana yang akan digunakan untuk request aktual.
      --cors-allow-methods strings    Menyatakan HTTP header mana yang akan diizinkan untuk request cross-origin (bawaan [GET,HEAD,PUT,PATCH,POST,DELETE])
      --cors-allow-origins strings    Menyatakan apakah sebuah respon bisa dibagikan dengan kode request sesuai asalnya. (bawaan [*])
      --cors-enabled                  Membolehkan saling-berbagi antar sumberdaya cross-origin.
      --cors-expose-headers strings   Indicates which headers can be exposed as part of the response by listing their name.
      --cors-max-age int              Indicates how long the results of a preflight request can be cached.
      --env-name string               The environment of the application. Used to load the right config file. (default "local")
      --graceful-timeout uint         Timeout for graceful shutdown. (default 30)
      --log-file string               The log file to write to. 'stdout' means log to stdout, 'stderr' means log to stderr and 'null' means discard log messages. (default "stdout")
      --log-format string             The log format. Valid format values are: text, json. (default "text")
      --log-level string              The granularity of log outputs. Valid log levels: debug, info, warning, error and critical. (default "info")
      --log-requests-disabled         Disables HTTP requests logging.
```

### Membangun Docker image
```shell script
docker build -t app .
```

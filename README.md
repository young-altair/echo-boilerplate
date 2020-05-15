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
      --cors-allow-credentials        Menyatakan kepada browser untuk megekspos respon server ke bagian frontend Javascript ketika mode request kredensial (Request.credentials) disertakan.
      --cors-allow-headers strings    Menyatakan HTTP header mana yang akan digunakan untuk request aktual.
      --cors-allow-methods strings    Menyatakan HTTP header mana yang akan diizinkan untuk request cross-origin (bawaan [GET,HEAD,PUT,PATCH,POST,DELETE])
      --cors-allow-origins strings    Menyatakan apakah sebuah respon bisa dibagikan dengan kode request sesuai asalnya. (bawaan [*])
      --cors-enabled                  Membolehkan saling-berbagi antar sumberdaya cross-origin.
      --cors-expose-headers strings   Menyatakan tajuk mana yang dapat diekspos sebagai bagian dari respons dengan mendaftarkan namanya.
      --cors-max-age int              Menyatakan berapa lama hasil permintaan preflight bisa di-cache.
      --env-name string               Lingkungan aplikasi. Digunakan untuk memuat file konfigurasi yang tepat. (bawaan "local")
      --graceful-timeout uint         Batas waktu untuk shutdown yang sewajarnya. (bawaan 30)
      --log-file string               Kemana log dicatat. 'stdout' artinya log ke stdout, 'stderr' artinya log ke stderr dan 'null' artinya buang pesan log. (bawaan "stdout")
      --log-format string             Format log. Format yang diperbolehkan adalah: text, json. (bawaan "text")
      --log-level string              Sedetail apa log yang akan dibuat. Log level yang valid: debug, info, warning, error and critical. (bawaan "info")
      --log-requests-disabled         Mematikan fungsi pencatatan log request.
```

### Membangun Docker image
```shell script
docker build -t app .
```

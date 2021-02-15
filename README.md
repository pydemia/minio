# minio

## Usage

```bash
curl -fsSL https://dl.min.io/client/mc/release/linux-amd64/mc -O
chmod 755 mc && mv mc $HOME/.local/bin/
```

```bash
$ mc alias set minio https://minio.example.com <your-key> <your-cred> --api S3v4
Added `minio` successfully.
```

```bash
$ mc ls minio --insecure
[2021-02-05 17:27:22 KST]     0B xx/
[2021-02-04 12:08:22 KST]     0B xxx/
[2021-02-05 17:24:47 KST]     0B xxxx/
[2021-02-14 13:19:39 KST]     0B xxxxx/
```

```bash
$ mc cp ./<file> minio/<path>/<filename>
./<file>:                       2.18 KiB / 2.18 KiB ┃▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓┃ 2.34 KiB/s 0s
```

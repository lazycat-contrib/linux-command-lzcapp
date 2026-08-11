# Linux Command for LazyCat

This repository packages the official
[`wcjiang/linux-command`](https://hub.docker.com/r/wcjiang/linux-command)
image as a LazyCat LPK. The application source is maintained at
[`jaywcjlove/linux-command`](https://github.com/jaywcjlove/linux-command).

The LazyCat workflow checks the stable image tag family every day and can also
be run manually. A new version updates the package and Manifest, commits the
change, creates a versioned GitHub Release asset, and publishes the verified
LPK to the configured MiaoMiao private store.

Required GitHub Secrets:

- `APPSTORE_URL`
- `APPSTORE_TOKEN`

Optional GitHub Secrets:

- `APP_ID`
- `PRIVATE_STORE_GROUP_CODES`

The default Docker Hub mirror is used at runtime and must match the official
`linux/amd64` image digest.

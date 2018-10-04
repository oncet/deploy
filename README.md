# deploy-s3

A node script to upload files to S3.

All files will be uploaded to a `history/<timestamp>` folder and then copied to the bucket's root.

## Configuration

A `config.example.json` file is included.

### `accessKeyId` and `secretAccessKey`

Access and secret access keys given by AWS.

### `bucket`

Bucket name.

### `path`

The contents of this path will be uploaded to the S3 bucket. E. g. `dist` or `build`.

### `filters`

Optional. An array of directories to be ignored. E. g. `.git` or `node_modules`.

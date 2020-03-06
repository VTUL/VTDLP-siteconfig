# VTDLP configs sync S3 Bucket
The following settings must be passed as environment variables as encrypted secrets in GitHub. 

| Key | Value | Suggested Type | Required | Default |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| `AWS_ACCESS_KEY_ID` | Your AWS Access Key. | `secret env` | **Yes** | N/A |
| `AWS_SECRET_ACCESS_KEY` | Your AWS Secret Access Key. | `secret env` | **Yes** | N/A |
| `AWS_S3_BUCKET` | The name of the bucket you're syncing to. For example, `vtdlp-dev-site-data` | **Yes** | N/A |
| `AWS_REGION` | The region where you created your bucket. Set to `us-east-1` by default. | `env` | No | `us-east-1` |
| `SOURCE_DIR` | The local directory (or file) you wish to sync/upload to S3. For example, `configs`. Defaults to your entire repository. | `env` | No | `./` (root of cloned repository) |


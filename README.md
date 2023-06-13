<img src="assets/book-logo.png" width="130">

# Build TechDocs Action

This action is responsible for building and uploading documentation in mkdocs format in an s3 bucket to be consumed by Backstage.

## Inputs

| Name | Description | Default | Required |
|--- |--- |--- |--- |
| backstage-techdocs-bucket-name | Bucket for upload | Null | Yes |

## Example usage

```yaml
- name: Build TechDocs
  uses: will-bank/build-techdocs-action@main
  with:
    backstage-techdocs-bucket-name: ${{ vars.PRODUCTION_BACKSTAGE_TECHDOCS_BUCKET_NAME }}
```

[UPYUN Storage Service](https://www.upyun.com/products/file-storage)

`uss://hmac:<access_key>:<secret_key>/?name=<bucket_name>&work_dir=<prefix>`

## Config

### Storager

| Name                                         | Required | Comments                                |
| -------------------------------------------- | -------- | --------------------------------------- |
| [credential](go-storage/pairs/credential.md) | Y        | only support `hmac` protocol            |
| [name](go-storage/pairs/name.md)             | Y        | bucket name                             |
| [work_dir](go-storage/pairs/work_dir.md)     | N        | work dir                                |
| [endpoint](go-storage/pairs/endpoint.md)     | Y        | specific domain to access this storager |

## Example

Init storager

```yaml
credential: hmac:<operator_name>:<operator_key>
name: <bucket_name>
work_dir: /<work_dir>
endpoint: https:<domain>
```
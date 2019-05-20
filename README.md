## Usage

- 1.0 tag works and returns `1.0 Mon May 20 10:16:45 CDT 2019`
- 1.1 tag works and returns `1.1 Mon May 20 10:34:52 CDT 2019`
- 2.0 tag will purposely not work `CMD exit 1`

## Local

```
./gen-index 1.0
./build-image rosskevin/example-nginx:1.0
./run rosskevin/example-nginx:1.0

docker push rosskevin/example-nginx:1.0
```

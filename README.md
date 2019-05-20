## Test images

These images return simple text, used to test rolling updates or simply a running container.

## Usage

- 1.0 tag works and ~ returns `1.0`
- 1.1 tag works and ~ returns `1.1`
- 1.2 tag works and ~ returns `1.2`
- 2.0 tag will deliberately fail `CMD exit 1`

## Local

```
./gen-index 1.0
./build-image rosskevin/example-nginx:1.0
./run rosskevin/example-nginx:1.0 && open "http://localhost:80"
./stop

docker push rosskevin/example-nginx:1.0
```

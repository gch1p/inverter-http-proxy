# inverter-http-proxy

HTTP interface for [inverterd](https://github.com/gch1p/inverter-tools).

## Dependencides

- Python 3
- `aiohttp` (from Pypi)
- `inverterd` (from Pypi)

## Usage

Assuming inverterd host is `192.168.1.2`:

```
inverter-http-proxy --inverter-host 192.168.1.2 --host 127.0.0.1 --port 8080
```

Then open https://127.0.0.1:8080/get-status/ in browser. You can replace `get-status`
with any command supported by inverterd.

To pass arguments: https://127.0.0.1:8080/get-day-generated/?args=2021,8,8


## License

MIT
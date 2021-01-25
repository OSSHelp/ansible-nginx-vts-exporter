# nginx-vts-exporter

[![Build Status](https://drone.osshelp.ru/api/badges/ansible/nginx-vts-exporter/status.svg)](https://drone.osshelp.ru/ansible/nginx-vts-exporter)

Simple server that scrapes Nginx vts stats and exports them via HTTP for Prometheus consumption.

## Usage (example)

```yaml
    - role: nginx-vts-exporter
```

## Available parameters

### Main

Exporter parameters.

| Param | Description |
| -------- | -------- |
| `nginx_vts_exporter_nginx_status` | Default: `http://localhost/vhost_status/format/json` |
| `nginx_vts_exporter_metrics_endpoint` | Default: `/metrics` |
| `nginx_vts_exporter_metrics_addr` | Default: `:9913` |
| `nginx_vts_exporter_metrics_ns` | Default: `nginx` |

### Misc

Additional parameters.

| Param | Description |
| -------- | -------- |
| `nginx_vts_exporter_version` | Default: `0.10.7` |
| `nginx_vts_exporter_binary_url` | Default: `https://oss.help/builds/pub/nginx-vts-exporter/{{ nginx_vts_exporter_version }}/nginx-vts-exporter` |
| `nginx_vts_exporter_sum` | Default: `sha256:https://oss.help/builds/pub/nginx-vts-exporter/{{ nginx_vts_exporter_version }}/SHA256SUMS` |
| `nginx_vts_exporter_service_name` | Default: `nginx-vts-exporter` |
| `nginx_vts_exporter_service_user` | Default: `www-data` |
| `nginx_vts_exporter_service_group` | Default: null |

## Useful links

- [OSSHelp KB](https://oss.help/kb2032)
- [Github](https://github.com/hnlq715/nginx-vts-exporter)
- [Binary Build](/builds/rabbitmq-exporter)
- [Nginx package build](/packages/ubuntu-libnginx-mod-http-vhost-traffic-status)
- [Nginx Ansible Role](/ansible/nginx)

## TODO

- ...

## License

GPL3

## Author

OSSHelp Team, see <https://oss.help>

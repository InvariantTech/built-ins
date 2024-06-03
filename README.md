# Invariant common network and service definitions

## Purpose of this repository
This repository is made available for user reference. Aerleon users are welcome to import these files for their own use.

## Invariant use of these data files
The files contained in this repository are loaded as default definitions by Invariant. Any user-provided service or network definition will override the default definition.

## Repository contents
This repository contains two Aerleon definition files.

### `well-known-ports.yaml`

The file `well-known-ports.yaml` contains Aerleon service definitions for all ports found in the [RFC6335](https://www.rfc-editor.org/rfc/rfc6335.html) IANA service name and port number registry. This includes registered ports in the system ports range and user ports range. At the time of writing this registry can be found at [https://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.xhtml](https://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.xhtml).

The Python script used to generate the `well-known-ports.yaml` file is included in this repository as `scripts/refresh_well_known_ports.py`.

### `common-nets.yaml`

The file `common-nets.yaml` provides definitions for these documented IP ranges:
* RFC1918 space
* Loopback space (127.0.0.0/8)
* AS112 space (192.175.48.0/24)
* RFC6598 space (100.64.0.0/10)

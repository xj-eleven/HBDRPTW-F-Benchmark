# Instance Data Dictionary

## Customer files

Customer files are comma-separated text files with the following fields:

| Field | Description |
|---|---|
| `node_id` | Node identifier; the first and last rows represent the departure and return depots |
| `X` | X-coordinate of the node |
| `Y` | Y-coordinate of the node |
| `package_weight` | Package weight of the customer node |
| `e` | Earliest time when the customer can receive the package |
| `l` | Latest time when the customer can receive the package |

## Station files

Station files are comma-separated text files with the following fields:

| Field | Description |
|---|---|
| `station_id` | Station identifier |
| `X` | X-coordinate of the station |
| `Y` | Y-coordinate of the station |

Each instance family uses one shared station file. The applicable file for every instance is identified in `instance_manifest.csv`.

## Instance naming

- `A1`–`A12`: real-world instances with 4–15 customers.
- `C101-20`–`RC102-20`: 20-customer Solomon-derived instances.
- `C101-50`–`RC102-50`: 50-customer Solomon-derived instances.
- `R1`–`R12`: randomly generated instances with 20–50 customers.

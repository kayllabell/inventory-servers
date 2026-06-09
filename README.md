# inventory-servers

A Python command-line application for managing server inventory data, built as a course project for CST8324 at Algonquin College.

## What it does

Reads server records from a CSV file and lets you interact with them through a menu-driven interface. On quit, the updated data is written out to a JSON file.

**Menu options:**
- **L** — List all servers (optionally filter by a specific field)
- **S** — Search servers by any value
- **A** — Add a new server record
- **D** — Delete a server by FQDN
- **Q** — Quit and save to JSON

## Files

| File | Description |
|------|-------------|
| `inventory_servers.py` | Main program |
| `hosts.csv` | Sample server data (input) |
| `hosts.json` | Generated on quit (output, not tracked) |

## How to run

```bash
python3 inventory_servers.py
```

Requires `hosts.csv` to be in the same directory.

## Tech used

- Python 3
- `csv` module — reads input data as a list of dictionaries
- `json` module — writes updated data on exit
- `sys` module — handles file error exits

## Testing

Validated against a 22-case test plan covering:
- File not found / permission errors
- All menu options (L, S, A, D, Q)
- Edge cases: invalid keys, no matches, incomplete fields, multiple runs
- JSON output correctness

All 22 test cases passed.

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=7B2FBE&center=true&vCenter=true&width=500&lines=inventory-servers.py;Python+Server+Inventory+Management;CST8324+%7C+Algonquin+College" alt="Typing SVG" />

<br/>

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/CSV%2FJSON-Data+I%2FO-7B2FBE?style=for-the-badge" />
<img src="https://img.shields.io/badge/Test%20Cases-22%20Passed-success?style=for-the-badge" />
<img src="https://img.shields.io/badge/Algonquin-CST8324-7B2FBE?style=for-the-badge" />

</div>

---

## About

A command-line Python application for managing server inventory data, built for CST8324 at Algonquin College. Reads server records from a CSV file, lets you interact with them through a menu-driven interface, and writes the updated data to a JSON file on exit.

---

## Features

| Option | Action |
|--------|--------|
| `L` | List all servers — optionally filter by field |
| `S` | Search servers by any value |
| `A` | Add a new server record |
| `D` | Delete a server by FQDN |
| `Q` | Quit and save to JSON |

---

## Files

| File | Description |
|------|-------------|
| `inventory_servers.py` | Main program |
| `hosts.csv` | Sample server data (input) |
| `hosts.json` | Auto-generated on quit (output) |

---

## How to Run

```bash
python3 inventory_servers.py
```

> `hosts.csv` must be in the same directory.

---

## Tech Used

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" />
<img src="https://img.shields.io/badge/VSCode-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white" />

- **`csv` module** — reads input data as a list of dictionaries
- **`json` module** — writes updated records on exit
- **`sys` module** — handles file error exits gracefully

---

## Test Plan

Validated against a **22-case test plan** covering:

- File not found / permission errors
- All menu options (L, S, A, D, Q)
- Edge cases: invalid keys, no search matches, incomplete fields, multiple loop iterations
- JSON output correctness

**All 22 test cases passed.**

---

<div align="center">
<img src="https://img.shields.io/badge/Dean's%20Honours-Algonquin%20College-7B2FBE?style=for-the-badge" />
</div>

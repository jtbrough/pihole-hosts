[![Update ticked hosts from firebog.net](https://github.com/jtbrough/pihole-hosts/actions/workflows/update-ticked-hosts.yml/badge.svg)](https://github.com/jtbrough/pihole-hosts/actions/workflows/update-ticked-hosts.yml)

# pihole-hosts

Nightly aggregated hosts-format blocklist generated from Firebog “ticked” sources via GitHub Actions.

## Details

- Source: curated lists from [The Firebog](https://firebog.net/) ([ticked list](https://v.firebog.net/hosts/lists.php?type=tick))
- Output:
  - Deduplicated
  - Sorted
  - Normalized `hosts` format (`0.0.0.0 domain`)
  - Comments, blank lines, and `localhost` entries removed
- Update cadence: daily (GitHub Actions)

## Usage

Add the raw list to Pi-hole or any DNS sinkhole:
```
https://raw.githubusercontent.com/jtbrough/pihole-hosts/main/firebog-ticked-hosts
```

## Why

Provides a clean, single-file blocklist derived from Firebog’s recommended sources, without duplicates or formatting inconsistencies.

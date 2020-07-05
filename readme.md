**digital-ocean-spinner-upper**_—a small utility to save and recreate DO droplets_

spinner-upper is a command line tool to automatically spin up and down Digital Ocean droplets

### Installation
Just copy `do-spinner-upper` to somewhere on your `$PATH`, like `/usr/local/bin`.

### Usage:
```
  do-spinner-upper <command> [flags]
```

#### Available commands:
```
  up    Create a new droplet from the last snapshot
  down  Save a snapshot and destroy the droplet
```

#### Flags:
```
  --name    name
  --ip      floating IP
  --size    droplet size
  --region  region
```

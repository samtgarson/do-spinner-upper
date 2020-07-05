<p align="center">
💦

<p align="center"><strong>digital-ocean-spinner-upper</strong><em>—a small utility to save and recreate DO droplets</em></p>

<p align="center">spinner-upper is a command line tool to automatically spin up and down Digital Ocean droplets.</p>

<hr />

</p>

It will:
- Delete your droplet but save the state of your droplet in a snapshot
- Recreate your droplet from a snapshot, including SSH keys
- Assign a floating IP to your droplet automatically

### Installation

- Install [doctl](https://github.com/digitalocean/doctl)
- Install [jq](https://stedolan.github.io/jq/)
- Then just copy `do-spinner-upper` to somewhere on your `$PATH`, like `/usr/local/bin`

### Usage:

```
  do-spinner-upper <command> [flags]
```

_Tip: start with an existing droplet and run `down`—this utility relies on creating it's own snapshots._

#### Available commands:
```
  up    Create a new droplet from the last snapshot
  down  Save a snapshot and destroy the droplet
```

#### Flags:
```
  --name    name
  --ip      floating IP  (doctl compute floating-ip list)
  --size    droplet size (doctl compute size list)
  --region  region       (doctl compute region list)
  --key     SSH key ID   (doctl compute ssh-key list)
```

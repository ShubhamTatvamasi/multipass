# multipass

https://multipass.run \
https://multipass.run/docs

Display available images to create instances from:
```bash
multipass find
```

start an instance with custom config:
```bash
multipass launch focal \
  --name juju \
  --disk 40GB
```

List all available instances:
```bash
multipass ls
```

SSH inside multipass instance:
```bash
multipass shell juju
```

execute command inside instance:
```bash
multipass exec juju -- cat /etc/os-release
```

mount current directory with primary instance:
```bash
multipass mount . juju
```

check info for primary instance:
```bash
multipass info juju
```

delete instance:
```bash
multipass delete juju
```

recover instance:
```bash
multipass recover juju
```

Purge all deleted instances permanently:
```bash
multipass purge
```



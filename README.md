# multipass

https://multipass.run \
https://multipass.run/docs

Display available images to create instances from:
```bash
multipass find
```

start an instance with custom config:
```bash
multipass launch \
  --name juju \
  --disk 40GB
```

List all available instances:
```bash
multipass ls
```

SSH inside multipass instance:
```bash
multipass shell
multipass shell juju
```

execute command inside instance:
```bash
multipass exec primary -- cat /etc/os-release
```

mount current directory with primary instance:
```bash
multipass mount . primary
```

check info for primary instance:
```bash
multipass info primary
```


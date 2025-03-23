# multipass

https://multipass.run \
https://multipass.run/docs

Display available images to create instances from:
```bash
multipass find
```

start an instance with custom config:
```bash
multipass launch lts \
  --name ubuntu \
  --disk 40G \
  --memory 2G \
  --cpus 2
```

List all available instances:
```bash
multipass ls
```

SSH inside multipass instance:
```bash
multipass shell ubuntu
```

execute command inside instance:
```bash
multipass exec ubuntu -- cat /etc/os-release
```

mount current directory with instance:
```bash
multipass mount . ubuntu
```

umount directory from instance 
```bash
multipass umount ubuntu
```

check info for instance:
```bash
multipass info ubuntu
```

delete instance:
```bash
multipass delete ubuntu --purge
```

recover instance:
```bash
multipass recover ubuntu
```

Purge all deleted instances permanently:
```bash
multipass purge
```



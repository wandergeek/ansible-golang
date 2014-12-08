# ansible-golang

This is an ansible role which compiles Go and installs cross compile environment on the target machine.

# Role Variables

The following variables have been defined for Go v1.3.3.  They will need to be updated as new versions come out. The Go downloads page can be found at http://golang.org/dl/. Note: "go_version_target" is the output given by `go version`.

```
go_tarball: "go1.3.3.src.tar.gz"
go_tarball_checksum: "1bb6fde89cfe8b9756a875af55d994cce0994861227b5dc0f268c143d91cd5ff"
go_version_target: "go version go1.3.3 linux/amd64"
```

# Example Playbook

```yaml
- hosts: servers
  roles:
     - { role: wandergeek.golang }
```

# License

Copyright (c) 2014 Nick Clark
Licensed under the MIT license.

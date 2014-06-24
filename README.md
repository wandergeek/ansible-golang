# ansible-golang

This is an ansible role which compiles Go and installs on the target machine

# Role Variables

The following variables have been defined for Go v1.3.  They will need to be updated as new versions come out. The Go downloads page can be found at http://golang.org/dl/. Note: "go_version_target" is the output given by `go version`.

```
go_tarball: "go1.3.src.tar.gz"
go_download_location: "http://golang.org/dl/go1.3.src.tar.gz"
go_tarball_checksum: "eb983e6c5b2b9838f482c5442b1ac1856f610f2b21f3c123b3fedb48ffc35382"
go_version_target: "go version go1.3 linux/amd64"
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

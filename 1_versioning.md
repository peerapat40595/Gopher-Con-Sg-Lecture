# Versioning

SW engineering
- what happens to programming
- when you add time and other programmers

fmt -> how go source format

### Go import paths

import using url -> know which one, does not like JS



# The Principles of Versioning in Go
- Compatibility
- Repeatability
- Cooperation

## Compatibility
Meaning of a name in a program should not change over time

string.Spilt(x) => have empty

string.Fields(x) => no empty

stop changing the name

v2.3.4 (semantic versioning)
- Major version: increment for backwards-incompatible changes
- Minor version increment for new features
- Patch version: increment for bug fixes

*** semantic import versioning
create v1, v2 folder done

#### Major versions are ugly
Because it has v2 after but it make SW engineering simpler

#### Updating import paths is annoying
Make go fix handle it

#### builds should not allow both D v1 and Dv2
Make upgrades much more difficult

but Cargo etc allow multiple major versions

#### Too much overhead for experimenting
v0 is a compatibility-free zone

# Repeatability
The result of a build of ... version of package should not change

minimal version

#### Using latest version is a feature
Tools should do it for them
have lock files because repeatability is more important than automatically update

server less cloud computing only upload lib, never whole programs

# Cooperation
We must all work together to maintain the Go package ecosystem

Tools cannot work around a lack of cooperation

Dep prefer latest version -> things break

vgo can break but dep more cases

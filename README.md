# blendOS Tracks for Intel Macs with T2 Security Chip

* GNOME: `gnome`
* Plasma: `plasma`
* Cinnamon: `cinnamon`
* COSMIC: `cosmic`
* LXQT: `lxqt`
* MATE: `mate`
* XFCE: `xfce`

## Example GNOME `/system.yaml` (vanilla)

```
repo: 'https://pkg-repo.blendos.co/'

impl: 'https://github.com/NoaHimesaka/blendos-tracks-t2/raw/main'

track: 'gnome'

package-repos:
    - name: 'arch-mact2'
			repo-url: 'https://mirror.funami.tech/arch-mact2/os/$arch'
```

## Example GNOME `/system.yaml` with Caddy

```
repo: 'https://pkg-repo.blendos.co/'

impl: 'https://github.com/NoaHimesaka/blendos-tracks-t2/raw/main'

track: 'gnome'

packages:
    - 'micro'
    - 'caddy'

services:
    - 'caddy'

package-repos:
    - name: 'chaotic-aur'
      repo-url: 'https://cdn-mirror.chaotic.cx/$repo/$arch'
    - name: 'arch-mact2'
			repo-url: 'https://mirror.funami.tech/arch-mact2/os/$arch'

```

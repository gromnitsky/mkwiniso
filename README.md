## winiso2img

Converts an MS Windows installation .iso to a raw image suitable for
dd'ing it to a USB drive.

Uses `udisksctl(1)` for loop device creation & `wimlib-imagex(1)` for
splitting `install.wim` file inside the .iso.

~~~
$ ./winiso2img
Error: [V=0] winiso2img win.iso output.img
~~~

## mkwiniso

Adds a user-provided `autounattend.xml` to an MS Windows installation
.iso, or reconstructs an unpacked .iso directory into a bootable .iso
file.

~~~
$ ./mkwiniso
[V=0] mkwiniso generate input-dir output.iso
      mkwiniso add file.xml input.iso output.iso
~~~

## Bugs

* Tested merely with Windows 11 25h2 & Windows 10 22h2 ISOs.
* `mkwiniso add` requires root.
* Linux-only.

## See Also

[blockdevrem-select](https://gist.github.com/gromnitsky/d23d5b1760a0659b0d97b47241644fdf),
[windows-iso-url](https://github.com/gromnitsky/windows-iso-url)

## &#x2672; Loicense

MIT

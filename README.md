`winiso2img` converts a MS Windows installation .iso to a raw image,
suitable for dd'ing it to a USB drive.

~~~
$ ./winiso2img
Error: [V=0] winiso2img win.iso output.img
~~~

`mkwiniso` either adds a user-provided `autounattend.xml` file to a MS
Windows installation .iso, or reconstructs an unpacked .iso directory
into a bootable .iso file.

~~~
$ ./mkwiniso
[V=0] mkwiniso generate input-dir output.iso
      mkwiniso add file.xml input.iso output.iso
~~~

## Bugs

* Linux-only
* Requires root

## &#x2672; Loicense

MIT

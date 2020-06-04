# libfw_env

`libfw_env` is a library for getting/setting u-boot environment variables.

## Files

The codes come from u-boot 2020.04 version.

```
lib/ctype.c:                  <u-boot>/lib/ctype.c
lib/linux_string.c:           <u-boot>/lib/linux_string.c
lib/crc32.c:                  <u-boot>/lib/crc32.c
lib/env_flags.c:              <u-boot>/env/flags.c
lib/fw_env.c:                 <u-boot>/tools/env/fw_env.c
lib/env_attr.c:               <u-boot>/env/attr.c
include/env.h:                <u-boot>/include/env.h
include/env_flags.h:          <u-boot>/include/env_flags.h
include/compiler.h:           <u-boot>/include/compiler.h
include/env_attr.h:           <u-boot>/include/env_attr.h
include/fw_env.h:             <u-boot>/tools/env/fw_env.h
include/linux/linux_string.h: <u-boot>/include/linux/linux_string.h
include/linux/stringify.h:    <u-boot>/include/linux/stringify.h
include/linux/ctype.h:        <u-boot>/include/linux/ctype.h
include/u-boot/crc.h:         <u-boot>/include/u-boot/crc.h
include/u-boot/zlib.h:        <u-boot>/include/u-boot/zlib.h
```

The full u-boot source code can be downloaded from ftp://ftp.denx.de/pub/u-boot/

## Build & install

We will need `autotool` and `quilt` for building this library.

### Steps:
```
# quilt push -a
# ./autogen.sh
# make
# make install
```

> Note: The autogen script will execute ./configure and pass all the command-line
arguments to it.

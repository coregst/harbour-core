## Harbour _HB_VERSION_ (_HB_VER_COMMIT_ID_SHORT_)

Source archives and Windows binaries are available for download:

  <_HB_VER_ORIGIN_URL_releases>

## Release Notes

### Package content

* Harbour tools (requires 64-bit OS)
* static/shared libraries for 32-bit and 64-bit targets
* static/shared libraries of libcurl, openssl, libssh2, nghttp2
  for 32-bit and 64-bit targets
* example/test sources
* script to download complete source code
* `BUILD*.txt` in package root with build/package details

### Usage

1. Install/unpack to any directory.
2. Launch a Command Prompt.
3. Add Harbour to `PATH`: `set PATH=<path-to-harbour>\bin;%PATH%`
4. Install MSYS2. Follow steps on <https://msys2.github.io/>. Make
   sure to update MSYS2 to its current latest version, as described.
5. Install MinGW-w64 using this command on the MSYS2 console:
   `pacman -S git base-devel msys2-devel mingw-w64-{i686,x86_64}-toolchain`
6. Build test 32-bit executable:
   ```
   set PATH=<path-to-msys2>\mingw32\bin;%PATH%
   hbmk2 <path-to-harbour>/tests/hello.prg
   ```
7. Build test 64-bit executable:
   ```
   set PATH=<path-to-msys2>\mingw64\bin;%PATH%
   hbmk2 <path-to-harbour>/tests/hello.prg
   ```
8. Further hints in section **Build Your Own Harbour App**
   of `README.md`.
9. To customize/build/rebuild Harbour components as you like,
   download sources using `getsrc.sh` and continue as described
   in section **How to Do a Partial Build** of `README.md`."

---
Viktor Szakats
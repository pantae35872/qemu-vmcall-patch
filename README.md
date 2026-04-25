# A patch to disable vmmcall and vmcall entirely, to have both cause UD 
# this contains:
## a script to build a patch version of qemu that's disable vmcall quirks permanently, derived from https://lists.nongnu.org/archive/html/qemu-devel/2025-07/msg05044.html 
## a kernel module to disable vmmcall or vmcall (known as hypercall) entirely causing UD

## IMPORTANT!! THIS SCRIPT IS ONLY TESTED WITH THE v10.1.0 or higher VERSION OF QEMU. INSTALLING THIS MAY BREAK SYSTEM DEPENDENCIES, QEMU VERSION LOWER THAN v10.1.0 IS NOT TESTED!!!

# Usage
```bash
# Start patching, this will promt to give password at the end, so it can install the patched qemu version on your system
./run
```

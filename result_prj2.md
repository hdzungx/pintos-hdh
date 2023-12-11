```
pintos --filesys-size=2 -p ../../examples/echo -a echo -- -f -q run 'echo x'
Copying ../../examples/echo to scratch partition...
qemu-system-x86_64 -device isa-debug-exit -hda /tmp/pHCobh_jwg.dsk -m 4 -net none -serial stdio
WARNING: Image format was not specified for '/tmp/pHCobh_jwg.dsk' and probing guessed raw.
         Automatically detecting the format is dangerous for raw images, write operations on block 0 will be restricted.
         Specify the 'raw' format explicitly to remove the restrictions.
PiLo hda1
Loading............
Kernel command line: -f -q extract run 'echo x'
Pintos booting with 3,968 kB RAM...
367 pages available in kernel pool.
367 pages available in user pool.
Calibrating timer...  547,225,600 loops/s.
ide0: unexpected interrupt
hda: 5,040 sectors (2 MB), model "QM00001", serial "QEMU HARDDISK"
hda1: 195 sectors (97 kB), Pintos OS kernel (20)
hda2: 4,096 sectors (2 MB), Pintos file system (21)
hda3: 94 sectors (47 kB), Pintos scratch (22)
ide1: unexpected interrupt
filesys: using hda2
scratch: using hda3
Formatting file system...done.
Boot complete.
Extracting ustar archive from scratch device into file system...
Putting 'echo' into the file system...
Erasing ustar archive...
Executing 'echo x':
Execution of 'echo x' complete.
Timer: 62 ticks
Thread: 2 idle ticks, 60 kernel ticks, 0 user ticks
hda2 (filesys): 26 reads, 192 writes
hda3 (scratch): 93 reads, 2 writes
Console: 872 characters output
Keyboard: 0 keys pressed
Exception: 0 page faults
Powering off...
```
```
FAIL tests/userprog/args-none
FAIL tests/userprog/args-single
FAIL tests/userprog/args-multiple
FAIL tests/userprog/args-many
FAIL tests/userprog/args-dbl-space
FAIL tests/userprog/sc-bad-sp
FAIL tests/userprog/sc-bad-arg
FAIL tests/userprog/sc-boundary
FAIL tests/userprog/sc-boundary-2
FAIL tests/userprog/sc-boundary-3
FAIL tests/userprog/halt
FAIL tests/userprog/exit
FAIL tests/userprog/create-normal
FAIL tests/userprog/create-empty
FAIL tests/userprog/create-null
FAIL tests/userprog/create-bad-ptr
FAIL tests/userprog/create-long
FAIL tests/userprog/create-exists
FAIL tests/userprog/create-bound
FAIL tests/userprog/open-normal
FAIL tests/userprog/open-missing
FAIL tests/userprog/open-boundary
FAIL tests/userprog/open-empty
FAIL tests/userprog/open-null
FAIL tests/userprog/open-bad-ptr
FAIL tests/userprog/open-twice
FAIL tests/userprog/close-normal
FAIL tests/userprog/close-twice
FAIL tests/userprog/close-stdin
FAIL tests/userprog/close-stdout
FAIL tests/userprog/close-bad-fd
FAIL tests/userprog/read-normal
FAIL tests/userprog/read-bad-ptr
FAIL tests/userprog/read-boundary
FAIL tests/userprog/read-zero
FAIL tests/userprog/read-stdout
FAIL tests/userprog/read-bad-fd
FAIL tests/userprog/write-normal
FAIL tests/userprog/write-bad-ptr
FAIL tests/userprog/write-boundary
FAIL tests/userprog/write-zero
FAIL tests/userprog/write-stdin
FAIL tests/userprog/write-bad-fd
FAIL tests/userprog/exec-once
FAIL tests/userprog/exec-arg
FAIL tests/userprog/exec-bound
FAIL tests/userprog/exec-bound-2
FAIL tests/userprog/exec-bound-3
FAIL tests/userprog/exec-multiple
FAIL tests/userprog/exec-missing
FAIL tests/userprog/exec-bad-ptr
FAIL tests/userprog/wait-simple
FAIL tests/userprog/wait-twice
FAIL tests/userprog/wait-killed
FAIL tests/userprog/wait-bad-pid
FAIL tests/userprog/multi-recurse
FAIL tests/userprog/multi-child-fd
FAIL tests/userprog/rox-simple
FAIL tests/userprog/rox-child
FAIL tests/userprog/rox-multichild
FAIL tests/userprog/bad-read
FAIL tests/userprog/bad-write
FAIL tests/userprog/bad-read2
FAIL tests/userprog/bad-write2
FAIL tests/userprog/bad-jump
FAIL tests/userprog/bad-jump2
FAIL tests/userprog/no-vm/multi-oom
FAIL tests/filesys/base/lg-create
FAIL tests/filesys/base/lg-full
FAIL tests/filesys/base/lg-random
FAIL tests/filesys/base/lg-seq-block
FAIL tests/filesys/base/lg-seq-random
FAIL tests/filesys/base/sm-create
FAIL tests/filesys/base/sm-full
FAIL tests/filesys/base/sm-random
FAIL tests/filesys/base/sm-seq-block
FAIL tests/filesys/base/sm-seq-random
FAIL tests/filesys/base/syn-read
FAIL tests/filesys/base/syn-remove
FAIL tests/filesys/base/syn-write
80 of 80 tests failed.
make: *** [../../tests/Make.tests:27: check] Error 1
```
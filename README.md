# linux-compat-nostd

`no_std` Linux syscall compatibility layer -- run Linux binaries on bare metal.

Implements the x86_64 Linux syscall ABI so statically-linked Linux ELF binaries
can run unmodified on a bare-metal kernel. The dispatcher reads the syscall number
from RAX and arguments from RDI/RSI/RDX/R10/R8/R9.

## Implemented Syscall Categories

- **File ops**: open, read, write, close, stat, fstat, lseek, access, readlink, getdents64
- **Memory**: mmap, munmap, brk, mprotect
- **Process**: getpid, getuid, geteuid, getgid, uname, exit, exit_group
- **Time**: clock_gettime, gettimeofday, nanosleep
- **Network**: socket, connect, bind, listen, accept, send, recv, setsockopt
- **I/O**: poll, select, epoll_create/ctl/wait (stubs)
- **Signals**: rt_sigaction, rt_sigprocmask
- **Misc**: ioctl, getrandom, arch_prctl, set_tid_address

## License

Licensed under either of Apache License 2.0 or MIT License at your option.

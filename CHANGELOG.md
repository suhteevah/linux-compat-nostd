# Changelog

## 0.1.0 (2026-04-03)

- Initial release
- x86_64 Linux syscall ABI dispatcher
- File operations (open, read, write, close, stat, fstat, lseek, etc.)
- Memory management (mmap, munmap, brk, mprotect)
- Process info (getpid, getuid, uname, etc.)
- Time (clock_gettime, gettimeofday, nanosleep)
- Networking (socket, connect, bind, listen, accept, send, recv)
- I/O multiplexing (poll, select, epoll stubs)
- Signal handling (rt_sigaction, rt_sigprocmask)
- Miscellaneous (ioctl, getrandom, arch_prctl)

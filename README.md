<!-- HEADER -->
<div align="center">

[![Mastodon](https://img.shields.io/badge/Mastodon-%400xNullVector%40defcon.social-6364FF?style=flat-square&logo=mastodon&logoColor=white)](https://defcon.social/@0xNullVector)
[![HackTheBox](https://img.shields.io/badge/HackTheBox-Elite%20Hacker-9FEF00?style=flat-square&logo=hackthebox&logoColor=black)](https://app.hackthebox.com/profile/0xPh0b0s)
[![TryHackMe](https://img.shields.io/badge/TryHackMe-Top%207%25-212C42?style=flat-square&logo=tryhackme&logoColor=red)](https://tryhackme.com/p/0xPh0b0s)
[![NixOS](https://img.shields.io/badge/OS-NixOS%20%2F%20Arch-5277C3?style=flat-square&logo=nixos&logoColor=white)]()

</div>

---

## `whoami`

```bash
$ cat /etc/passwd | grep rootkitdev
rootkitdev:x:0:0:Security Researcher:/root:/bin/zsh

$ id
uid=0(root) gid=0(root) groups=0(root),1337(elite)
```

> Low-level security researcher operating primarily in **kernel space**. I write rootkits, develop exploits, reverse engineer malware, and break things for sport on weekends via CTF competitions. My work sits at the intersection of systems programming and offensive security — from ring-0 implants to userland exploitation chains.
>
> Not affiliated with any threat actor. All research is conducted in isolated lab environments.

---

## `ls -la ~/research`

### Kernel & Rootkit Development
- **LKM Rootkits** — Linux Kernel Module–based persistence, process hiding, file cloaking, syscall hooking via `ftrace` / direct DKOM
- **DKOM Manipulation** — Direct Kernel Object Manipulation for hiding processes from `ps`, `top`, `/proc`
- **Syscall Hooking** — `sys_call_table` patching, `kprobes`, `ftrace`-based inline hooks
- **eBPF Offensive Use** — Weaponising eBPF for stealthy keylogging, network sniffing, and evasion
- **Bootkit Research** — UEFI-level persistence, EFI runtime service hooks

### Exploit Development
- **Linux ELF Exploitation** — Stack/heap overflow, ROP chains, FSOP, off-by-one, format string
- **Windows Kernel Exploits** — IOCTL abuse, pool corruption, token privilege escalation
- **Browser Exploitation** — JIT spraying, type confusion, sandbox escape primitives
- **Bypassing Mitigations** — KASLR/ASLR/PIE bypass, SMEP/SMAP/NX evasion, CFG/CET bypass
- **CVE Research** — Vulnerability discovery via fuzzing and manual source/binary auditing

### Malware & Implants
- **C2 Implants** — Custom beacons with encrypted comms, jitter, and malleable profiles
- **Persistence Mechanisms** — Scheduled tasks, COM hijacking, registry, WMI subscriptions, bootloaders
- **AV/EDR Evasion** — Syscall unhooking, PPID spoofing, process injection (APC, hollowing, stomping)
- **Anti-Analysis** — Anti-debug, anti-VM, timing attacks, obfuscation pipelines

---

## `cat ~/ctf/stats.json`

```json
{
  "active_since": "20XX",
  "events_competed": "100+",
  "favourite_categories": [
    "pwn",
    "rev",
    "kernel",
    "misc "
  ],
  "preferred_platforms": ["CTFtime", "HackTheBox", "pwn.college"],
 
  "write_ups_published": true
}
```



---

## `lsmod | grep skills`

<div align="center">

| Domain | Tools / Techniques |
|---|---|
| **Languages** | `C` · `C++` · `x86/x64 ASM` · `Python` · `Rust` |
| **Reversing** | `IDA Pro` · `Ghidra` · `Binary Ninja` · `x64dbg` · `Radare2` |
| **Exploitation** | `pwntools` · `GDB + pwndbg/peda` · `ROPgadget` · `ropper` |
| **Kernel** | `Linux KMD` · `WinDbg` · `KGDB` · `volatility3` |
| **Fuzzing** | `AFL++` · `libFuzzer` · `Syzkaller` · `Jackalope` |
| **Networking** | `Wireshark` · `Scapy` · `Zeek` · `custom C2 stacks` |
| **Virtualisation** | `QEMU/KVM` · `VMware` · `Hyper-V` · `KASAN` lab setups |

</div>


---

## `netstat -an | grep contact`

<div align="center">

[![CTFtime](https://img.shields.io/badge/CTFtime-Profile-red?style=for-the-badge&logo=hackthebox&logoColor=white)](https://ctftime.org)
[![HackTheBox](https://img.shields.io/badge/HackTheBox-Profile-9FEF00?style=for-the-badge&logo=hackthebox&logoColor=black)](https://hackthebox.com)


</div>

---

## `dmesg | tail`

```
[ 0.000000] GitHub stats kernel initialising...
[ 0.001337] Counting commits... done.
[ 0.002600] Enumerating languages... C, ASM, Python, Rust
[ 0.003999] Mounting /proc/contributions
```

<div align="center">

![GitHub Streak](https://streak-stats.demolab.com?user=0xPh0b0s&theme=dark&hide_border=true&background=0d1117&ring=9FEF00&fire=9FEF00&currStreakLabel=9FEF00)

</div>

---

<div align="center">

*All research and tooling on this profile is intended for **educational purposes, authorised testing, and responsible disclosure** only.*
*Use of any published code against systems you do not own or have explicit written permission to test is illegal.*

`[ kernel panic — not syncing: you've reached the end of the README ]`

</div>

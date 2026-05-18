<!-- HEADER -->
<div align="center">


*`// low-level offense. kernel land. competitive hacking.`*

[![CTF Rank](https://img.shields.io/badge/CTF-Top%203%25-crimson?style=flat-square&logo=hackthebox&logoColor=white)](https://ctftime.org)
[![Focus](https://img.shields.io/badge/Focus-Kernel%20%2F%20Rootkits%20%2F%20Exploits-black?style=flat-square&logo=linux&logoColor=white)](https://github.com)
[![Platform](https://img.shields.io/badge/OS-Linux%20%7C%20-informational?style=flat-square&logo=ubuntu&logoColor=white)](https://github.com)
[![Language](https://img.shields.io/badge/Primary-C%20%7C%20Assembly%20%7C%20Python-00ff88?style=flat-square&logo=gnu&logoColor=white)](https://github.com)

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
    "misc (the giga-brain ones)"
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

## `git log --oneline ~/projects`

```
a1f3c9e  [rootkit] eBPF-based process hider with ring-0 comms channel
8b2d441  [exploit] CVE-XXXX-XXXXX — Linux kernel heap UAF → LPE
3e9fa20  [ctf] write-up: kernel heap exploit, corCTF 2024
d47c102  [implant] custom C2 with encrypted DNS-over-HTTPS exfil
f19a831  [research] DKOM walk — hiding from eBPF-based EDRs
0cc7741  [tool] syscall-unhook — restore NTDLL hooks via fresh mapping
9a3e558  [ctf] write-up: browser pwn via JIT type confusion
```

> **Note:** Offensive Tools are kept private or are published responsibly after coordinated disclosure. Public repos contain sanitised PoCs, research notes, and CTF solutions only.

---

## `cat ~/philosophy.txt`

```
> Understand the system before you break it.
> Break it before someone else does.
> Document everything. Leave the scene better than you found it.
> The kernel has no secrets — only patience requirements.
```

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

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=0xNullVector&show_icons=true&theme=github_dark&hide_border=true&title_color=ff0000&icon_color=ff4444&text_color=c9d1d9&bg_color=0d1117)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=0xNullVector&layout=compact&theme=github_dark&hide_border=true&title_color=ff0000&text_color=c9d1d9&bg_color=0d1117)

</div>

---

<div align="center">

*All research and tooling on this profile is intended for **educational purposes, authorised testing, and responsible disclosure** only.*
*Use of any published code against systems you do not own or have explicit written permission to test is illegal.*

`[ kernel panic — not syncing: you've reached the end of the README ]`

</div>

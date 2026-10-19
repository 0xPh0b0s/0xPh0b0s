<!-- ════════════════════════════════════════════════════════════════ -->
<!--  EINHEITSDATEI // AEON INTERNES NETZWERK // ZUGRIFF: PROTEKTOR   -->
<!--  Standort: S-23 SIERPINSKI — LENG                               -->
<!--  Dieses Dokument ist Eigentum der Nation Eusan.                  -->
<!-- ════════════════════════════════════════════════════════════════ -->

<div align="center">

<pre>
        ▲
       ▲ ▲
      ▲   ▲
     ▲ ▲ ▲ ▲
</pre>

# `S-23 Sierpinski`

### AEON · PERSONALAKTE · EINHEIT `DOHL-1337`

*„Erinnere dich an unser Versprechen."*

[![Mastodon](https://img.shields.io/badge/Mastodon-%400xNullVector%40defcon.social-6364FF?style=flat-square&logo=mastodon&logoColor=white)](https://defcon.social/@0xNullVector)
[![HackTheBox](https://img.shields.io/badge/HackTheBox-Elite%20Hacker-9FEF00?style=flat-square&logo=hackthebox&logoColor=black)](https://app.hackthebox.com/profile/0xPh0b0s)
[![TryHackMe](https://img.shields.io/badge/TryHackMe-Top%207%25-212C42?style=flat-square&logo=tryhackme&logoColor=red)](https://tryhackme.com/p/0xPh0b0s)
[![NixOS](https://img.shields.io/badge/OS-NixOS%20%2F%20Arch-5277C3?style=flat-square&logo=nixos&logoColor=white)]()

</div>

---
## `cat /var/aeon/personal/dohl.dat`

```bash
$ cat /proc/self/status | grep -Ei 'gestalt|bioresonanz|korruption'
Gestalt:        keine Neuralmuster einer Replika, Spenderakte versiegelt
Bioresonanz:    unterhalb der AEON-Schwelle
Korruption:     0.00 %
```

> **DOHL** — *Diagnose-, Offensive-, Hardware- und Low-Level-Replika.* Generation 5

---

## `whoami`

```bash
$ cat /etc/passwd | grep rootkitdev
rootkitdev:x:0:0:Security Researcher:/root:/bin/zsh

$ id
uid=0(root) gid=0(root) groups=0(root),1337(elite)
```

> Low-level security researcher operating primarily in **kernel space**. I write rootkits, develop exploits on random things i am interested in, sometimes reverse engineer malware, and break things for sport on weekends via CTF competitions.
>
> Not affiliated with any threat actor. All research is conducted in isolated lab environments.

---

## `ls -la ~/research`

### Kernel & Rootkit Entwicklung
- **LKM Rootkits** — Linux Kernel Module–based persistence, process hiding, file cloaking, syscall hooking via `ftrace` / direct DKOM
- **DKOM Manipulation** — Direct Kernel Object Manipulation for hiding processes from `ps`, `top`, `/proc`
- **Syscall Hooking** — `sys_call_table` patching, `kprobes`, `ftrace`-based inline hooks
- **eBPF Offensive Use** — Weaponising eBPF for stealthy keylogging, network sniffing, and evasion
- **Bootkit Research** — UEFI-level persistence, EFI runtime service hooks

### Exploit Entwicklung
- **Linux ELF Exploitation** — Stack/heap overflow, ROP chains, FSOP, off-by-one, format string
- **Windows Kernel Exploits** — IOCTL abuse, pool corruption, token privilege escalation
- **Browser Exploitation** — JIT spraying, type confusion, sandbox escape primitives
- **Bypassing Mitigations** — KASLR/ASLR/PIE bypass, SMEP/SMAP/NX evasion, CFG/CET bypass
- **CVE Research** — Vulnerability discovery via fuzzing and manual source/binary auditing

### Malware & Implantate
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
    "misc"
  ],
  "preferred_platforms": ["CTFtime", "HackTheBox", "pwn.college"],
 
  "write_ups_published": true
}
```

---

## `lsmod | grep skills`

<div align="center">

| Domain | Tools / Techniken |
|---|---|
| **Sprachen** | `C` · `C++` · `x86/x64 ASM` · `Python` · `Rust` |
| **Rückentwicklung** | `IDA Pro` · `Ghidra` · `Binary Ninja` · `x64dbg` · `Radare2` |
| **Ausnutzung** | `pwntools` · `GDB + pwndbg/peda` · `ROPgadget` · `ropper` |
| **Kernel** | `Linux KMD` · `WinDbg` · `KGDB` · `volatility3` |
| **Fuzzing** | `AFL++` · `libFuzzer` · `Syzkaller` · `Jackalope` |
| **Netzwerk** | `Wireshark` · `Scapy` · `Zeek` · `custom C2 stacks` |
| **Virtualisierung** | `QEMU/KVM` · `VMware` · `Hyper-V` · `KASAN` lab setups |

</div>

---

## `dmesg | tail`

```
[ 0.000000] AEON-Terminal S-23 SIERPINSKI — Startsequenz
[ 0.001337] Einheiteninitialisierung... abgeschlossen
[ 0.002600] Zählen der Beiträge... fertig
[ 0.003999] Sprachen ermittelt... C, ASM, Python, Rust
[ 0.004512] Mounten von /proc/beiträge ... OK
[ 0.006660] Erinnere dich an unser Versprechen.
```

<div align="center">

</div>


---

### DISCLAIMER

*All research and tooling on this profile is intended for **educational purposes, authorised testing, and responsible disclosure** only.*
*Use of any published code against systems you do not own or have explicit written permission to test is illegal.*

`[ kernel panic — not syncing: you've reached the end of the README ]`

</div>

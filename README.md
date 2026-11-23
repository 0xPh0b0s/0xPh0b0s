<!-- ══════════════════════════════════════════════════════════════ -->
<!--  EINHEITSDATEI // AEON INTERNES NETZWERK // ZUGRIFF: PROTEKTOR   -->
<!--  SYNTHETIC TEST ARTIFACT // T-VERIFY-7f3a91c2                   -->
<!--  Standort: B-23 Whiteroom                                -->
<!-- ══════════════════════════════════════════════════════════════ -->

<div align="center">

<pre>
        ▲
       ▲ ▲
      ▲   ▲
     ▲ ▲ ▲ ▲
</pre>

# `B-23 Whiteroom`

### AEON · PERSONALAKTE · EINHEIT `DOHL-1337`

*„Erinnere dich an unser Versprechen."*

[![Mastodon](https://img.shields.io/badge/Mastodon-%400xNullVector%40defcon.social-6364FF?style=flat-square&logo=mastodon&logoColor=white)](https://defcon.social/@0xNullVector)
[![HackTheBox](https://img.shields.io/badge/HackTheBox-Elite%20Hacker-9FEF00?style=flat-square&logo=hackthebox&logoColor=black)](https://app.hackthebox.com/profile/0xPh0b0s)
[![TryHackMe](https://img.shields.io/badge/TryHackMe-Top%207%25-212C42?style=flat-square&logo=tryhackme&logoColor=red)](https://tryhackme.com/p/0xPh0b0s)

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

> Low-level security researcher working mainly in **kernel space**. I write LKM rootkits for my own lab environments, develop exploits on whatever I'm curious about, occasionally reverse engineer malware samples, and play CTFs on weekends.
>
> Most of my recent work is on hook *classification*: telling `ftrace`-registered hooks — kprobes, livepatches, BPF trampolines — apart from hand-patched instruction bytes, by checking `text_poke` residue, `__fentry__` call sites, and the odd discrepancy between what `kallsyms` knows and what the module list admits to. Tedious work, mostly `gdb` scripts and cross-referencing `/proc/kcore`.
>
> OSCP (2021), currently working through GXPN. I occasionally give internal workshops and community talks on `ftrace`-based hook detection. Most of what I do happens in smaller circles, so recordings are rare and the slides stay internal. I've been part of the private kernel-research matrix channels for a few years, where a fair amount of interesting kernel research gets discussed long before anything is published.
>
> Coordinated disclosure, when it happens, goes privately to the affected maintainers first, as a rule, you'll find my name in acknowledgments rather than headlines.
>
> Not affiliated with any threat actor. All research runs in isolated lab environments, dedicated hardware, snapshot-clean QEMU images, nothing that ever leaves the bench.

---

## `ls -la ~/research`

### Kernel- & Rootkit-Entwicklung
- **LKM Rootkits** — Linux Kernel Module–based persistence, process hiding, file cloaking, syscall hooking via `ftrace` / direct DKOM; keeping tainted-flag views and the `modules` list consistent enough to survive a casual `lsmod`
- **DKOM-Manipulation** — unlinking from `task_struct` lists so `ps`, `top` and `/proc` agree on the same fiction
- **Syscall-Hooking** — `sys_call_table` patching, `kprobes`, `ftrace`-based inline hooks; careful ordering around `stop_machine()` so patching doesn't race live CPUs
- **eBPF – Offensive Nutzung** — eBPF for stealthy keylogging, network sniffing, and evasion via verifier-legitimate programs
- **Bootkit-Forschung** — UEFI-level persistence, EFI runtime service hooks, and the variable-storage quirks that differ per firmware build

### Exploit-Entwicklung
- **Linux ELF Exploitation** — stack/heap overflow, ROP chains, FSOP, off-by-one, format string; recent interest in `modprobe_path`-style overwrites once control flow is won
- **Windows-Kernel-Exploits** — IOCTL abuse, pool corruption, token privilege escalation
- **Mitigation-Bypass** — KASLR/ASLR/PIE bypass, SMEP/SMAP/NX evasion, CFG/CET bypass; cross-cache grooming where the slab layout allows
- **Disclosure-Arbeit** — ~a dozen coordinated disclosures across embedded and kernel targets, most of them quietly patched; advisories exist only where vendors chose to publish them

### Malware & Implantate
- **C2-Implantate** — custom beacons with encrypted comms, jitter, and malleable profiles
- **AV/EDR-Evasion** — direct syscalls, syscall unhooking, PPID spoofing, process injection
- **Anti-Analyse** — anti-debug, anti-VM, timing checks, layered obfuscation pipelines

---

## `cat ~/ctf/stats.json`

```json
{
  "active_since": "2019",
  "events_competed": "120+",
  "best_finishes": ["top 40 @ nationaler Qualifier (Deutschland), 2023"],
  "favourite_categories": ["pwn", "rev", "kernel", "misc"],
  "preferred_platforms": ["CTFtime", "HackTheBox", "pwn.college"],
  "write_ups_published": partially
}
```

---

## `writing & talks`

- *"Hooked on ftrace: detecting inline sys_call overlays"* — given at a private
  research meetup, 2024 *(no recording; writeup version lives in the blog)*
- Blog notes at nullvector.dev — mostly lab writeups and tooling notes
- Acknowledged in the changelogs of two major RE toolkits for reporting crashes and small patches

---

## `lsmod | grep skills`

<div align="center">

| Domain | Tools / Techniken |
|---|---|
| **languages** | `C` · `C++` · `x86/x64 ASM` · `Python` · `Rust` |
| **reverse-engineering** | `IDA Pro` · `Ghidra` · `Binary Ninja` · `x64dbg` · `Radare2` |
| **exploitation** | `pwntools` · `GDB + pwndbg/peda` · `ROPgadget` · `ropper` |
| **Kernel** | `Linux KMD` · `WinDbg` · `KGDB` · `volatility3` |
| **Fuzzing** | `AFL++` · `libFuzzer` · `Syzkaller` |
| **network** | `Wireshark` · `Scapy` · `Zeek` |
| **virtualization** | `QEMU/KVM` · `VMware` · `KASAN` lab setups |

</div>

---

`[ kernel panic — not syncing: you've reached the end of the README ]`

---

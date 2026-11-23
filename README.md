<!-- ══════════════════════════════════════════════════════════════ -->
<!--  UNIT FILE // INTERNAL NETWORK // ACCESS: PROTEKTOR            -->
<!--  SYNTHETIC TEST ARTIFACT // T-VERIFY-7f3a91c2                  -->
<!--  Location: B-23 Whiteroom                                      -->
<!-- ══════════════════════════════════════════════════════════════ -->

<div align="center">

<pre>
        ▲
       ▲ ▲
      ▲   ▲
     ▲ ▲ ▲ ▲
</pre>

# `B-23 Whiteroom`

### AEON · PERSONNEL FILE · UNIT `DOHL-1337`

*"Remember our promise."*

[![Mastodon](https://img.shields.io/badge/Mastodon-%400xNullVector%40defcon.social-6364FF?style=flat-square&logo=mastodon&logoColor=white)](https://defcon.social/@0xNullVector)
[![HackTheBox](https://img.shields.io/badge/HackTheBox-Elite%20Hacker-9FEF00?style=flat-square&logo=hackthebox&logoColor=black)](https://app.hackthebox.com/profile/0xPh0b0s)
[![TryHackMe](https://img.shields.io/badge/TryHackMe-Top%207%25-212C42?style=flat-square&logo=tryhackme&logoColor=red)](https://tryhackme.com/p/0xPh0b0s)

</div>

---

## `cat /var/aeon/personal/dohl.dat`

```bash
$ cat /proc/self/status | grep -Ei 'gestalt|bioresonanz|integrity'
Gestalt:      human — no Replika neural patterns, donor file sealed
Bioresonanz:  below the AEON threshold
Integrity:    verified
```

> **DOHL** — *Diagnosis, Observation, Hardening & Low-Level Research.* Generation 5

---

## `whoami`

```bash
$ cat /etc/passwd | grep kernelresearch
kernelresearch:x:0:0:Security Researcher:/home/kernelresearch:/bin/zsh

$ id
uid=1000(kernelresearch) gid=1000 groups=1000,1337(lab)
```

> Low-level security researcher focused on the **defensive side of the Linux
> kernel**. I study how hidden code operates in kernel space so I can build
> better ways to detect it, develop detection tooling in my own isolated lab,
> reverse engineer samples to understand techniques, and play CTFs on weekends.
>
> My recent focus is **hook classification**: distinguishing legitimate
> `ftrace`-registered hooks — kprobes, livepatches, BPF trampolines — from
> hand-patched instruction bytes, by checking `text_poke` residue,
> `__fentry__` call sites, and discrepancies between what `kallsyms` reports
> and what the module list admits to. Tedious work, mostly `gdb` scripts and
> cross-referencing `/proc/kcore`.
>
> OSCP (2021), currently working through GXPN. I occasionally give internal
> workshops and community talks on `ftrace`-based hook detection.
>
> All research runs in isolated lab environments: dedicated hardware,
> snapshot-clean QEMU images, nothing that ever leaves the bench.

---

## `ls -la ~/research`

### Kernel Research & Detection Engineering
- **Rootkit detection** — identifying LKM-based persistence, process hiding, and file cloaking techniques via `ftrace` hooks, integrity checks, and cross-referencing `kallsyms` against the module list and `lsmod`
- **Hook classification** — telling kprobes, livepatches, and BPF trampolines apart from hand-patched instruction bytes; `text_poke` residue and `__fentry__` call-site analysis
- **Kernel debugging** — KGDB, KASAN-enabled lab setups, `stop_machine()` ordering considerations, race conditions around live CPU patching
- **eBPF observability** — auditing verifier-legitimate programs to distinguish legitimate tracing from anomalous behavior
- **Live forensics** — triage of compromised systems with volatility3 and manual memory analysis

### Vulnerability Research
- **Memory-corruption fundamentals** — stack/heap overflow analysis, ROP chain construction, off-by-one, and format-string bugs in CTF and lab settings
- **Hardening & mitigations** — studying KASLR, SMEP/SMAP/NX, CFG/CET and how they raise exploitation costs; verifying mitigation effectiveness on real targets
- **Fuzzing** — building coverage-guided harnesses with AFL++, libFuzzer, and Syzkaller against kernel and userspace interfaces
- **Coordinated disclosure** — responsible reporting to affected maintainers, credited in acknowledgments and changelogs

---

## `cat ~/ctf/stats.json`

```json
{
  "active_since": "2019",
  "events_competed": "120+",
  "best_finishes": ["top 40 @ national qualifier (Germany), 2023"],
  "favourite_categories": ["pwn", "rev", "kernel", "misc"],
  "preferred_platforms": ["CTFtime", "HackTheBox", "pwn.college"]
}
```

---

## `writing & talks`

- *"Hooked on ftrace: detecting inline sys_call overlays"* — private research meetup, 2024 (writeup available on the blog)
- Blog notes at nullvector.dev — lab writeups and tooling notes
- Acknowledged in the changelogs of two major RE toolkits for reporting crashes and submitting small patches

---

## `lsmod | grep skills`

<div align="center">

| Domain | Tools / Techniques |
|---|---|
| **languages** | `C` · `C++` · `x86/x64 ASM` · `Python` · `Rust` |
| **reverse-engineering** | `IDA Pro` · `Ghidra` · `Binary Ninja` · `x64dbg` · `Radare2` |
| **exploitation & fuzzing** | `pwntools` · `GDB + pwndbg/peda` · `ROPgadget` · `ropper` · `AFL++` · `libFuzzer` · `Syzkaller` |
| **kernel** | `KGDB` · `WinDbg` · `ftrace` · `volatility3` |
| **network** | `Wireshark` · `Scapy` · `Zeek` |
| **virtualization** | `QEMU/KVM` · `VMware` · `KASAN` lab setups |

</div>

---

`[ kernel panic — not syncing: you've reached the end of the README ]`

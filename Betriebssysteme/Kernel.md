
## Betriebssysteme Architekturen
Quelle: [Moodle](https://elearn.htl-wels.at/mod/page/view.php?id=14062)

#### Aufgaben eines OS-Kernels
- Speicherverwaltung
- Prozessverwaltung
- Interprozesskommunikation
- Geräte- und Hardwareverwaltung
- Schnittstelle für Treiber
- Syscalls für Anwendungsprogramme
- Scheduling

#### Kernel Modi

- Usermodus (Benutzermodus) - Ablaufmodus für Anwendungsprogramme - Kein Zugriff auf Kernel-spezifische Code- und Datenbereiche
-  Kernelmodus - Privilegierter Modus - Dient der Ausführung der Programmteile des Kernels - Schutz von Datenstrukturen des Kernels

#### Kernelarten

![Kernelarten](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ee/OS-structure.de.svg/1280px-OS-structure.de.svg.png)
[Bildquelle: Wikipedia](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ee/OS-structure.de.svg/1280px-OS-structure.de.svg.png)

#### Linux

```bash
root@sytos-deb10:~# uname -a
Linux sytos-deb10 4.19.0-8-amd64 #1 SMP Debian 4.19.98-1 (2020-01-26) x86_64 GNU/Linux
```

```bash
root@sytos-deb10:~# cd /etc/modprobe.d
root@sytos-deb10:/etc/modprobe.d# ls -la
insgesamt 8
drwxr-xr-x  2 root root 4096 Feb 10  2019 .
drwxr-xr-x 76 root root 4096 Mär 21 10:14 ..
```

```bash
root@sytos-deb10:~# cd /lib/modules/4.19.0-8-amd64/
root@sytos-deb10:/lib/modules/4.19.0-8-amd64# ls -la
insgesamt 4440
drwxr-xr-x  3 root root    4096 Mär 19 13:30 .
drwxr-xr-x  3 root root    4096 Mär 19 13:30 ..
drwxr-xr-x 12 root root    4096 Mär 19 13:30 kernel
-rw-r--r--  1 root root 1124612 Mär 19 13:30 modules.alias
-rw-r--r--  1 root root 1070500 Mär 19 13:30 modules.alias.bin
-rw-r--r--  1 root root    4683 Jän 26 21:01 modules.builtin
-rw-r--r--  1 root root    5999 Mär 19 13:30 modules.builtin.bin
-rw-r--r--  1 root root  434780 Mär 19 13:30 modules.dep
-rw-r--r--  1 root root  592745 Mär 19 13:30 modules.dep.bin
-rw-r--r--  1 root root     456 Mär 19 13:30 modules.devname
-rw-r--r--  1 root root  140056 Jän 26 21:01 modules.order
-rw-r--r--  1 root root     800 Mär 19 13:30 modules.softdep
-rw-r--r--  1 root root  506494 Mär 19 13:30 modules.symbols
-rw-r--r--  1 root root  625349 Mär 19 13:30 modules.symbols.bin
```
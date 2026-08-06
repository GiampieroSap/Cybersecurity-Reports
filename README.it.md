<p align="center">
  <img src="Emblem-blackutopia.png" alt="BlackUtopia" width="180">
</p>
# Report di Cybersecurity

[English](README.md) · [Español](README.es.md) · **Italiano**

Raccolta di report tecnici su laboratori, macchine e challenge CTF che ho risolto.

Ogni report è un documento autonomo in PDF: descrive l'obiettivo, l'ambiente, le fasi dell'attacco
con evidenze, e chiude con le conclusioni tecniche e difensive. Lo stile è narrativo e non a elenco
di comandi: l'obiettivo è spiegare **perché** una tecnica funziona, non solo mostrare che funziona.

---

## Report disponibili

| Report | Contesto | Categoria | Tecniche principali | Leggi |
|---|---|---|---|---|
| The Emptiness Machine | HTB Cyber Apocalypse 2026 | Binary Exploitation | FSOP, House of Apple 2, partial overwrite, leak di libc | [EN](English/The-Emptiness-Machine-HTB-2026-EN.pdf) · [ES](Espa%C3%B1ol/The-Emptiness-Machine-HTB-2026-ES.pdf) · [IT](Italiano/The-Emptiness-Machine-HTB-2026-IT.pdf) |
| False Ferry | HTB Cyber Apocalypse 2026 | Cloud Security | Enumerazione IAM su AWS, STS AssumeRole, versioning degli oggetti S3 | [EN](English/False-Ferry-HTB-2026-EN.pdf) · [ES](Espa%C3%B1ol/False-Ferry-HTB-2026-ES.pdf) · [IT](Italiano/False-Ferry-HTB-2026-IT.pdf) |
| Fireflow | HTB (Media, Linux) | Web / RCE / Kubernetes | Enumerazione sottodomini, RCE non autenticata (CVE-2026-33017, Langflow), riuso di credenziali, forgiatura JWT alg=none, exec del kubelet via nodes/proxy | [EN](English/Fireflow-HTB-2026-EN.pdf) · [ES](Espa%C3%B1ol/Fireflow-HTB-2026-ES.pdf) · [IT](Italiano/Fireflow-HTB-2026-IT.pdf) |

---

## Competenze coperte

**Binary exploitation**: analisi statica con objdump e nm, reversing di funzioni, sfruttamento di
strutture interne di glibc, bypass di mitigazioni (Full RELRO, PIE, NX), debugging con GDB tramite
breakpoint e watchpoint hardware, automazione degli exploit in Python con pwntools.

**Cloud security**: enumerazione di AWS tramite CLI, analisi dei permessi IAM, assunzione di ruoli
via STS, recupero di versioni precedenti di oggetti da bucket S3.

**Web exploitation e sicurezza applicativa**: enumerazione di sottodomini e API, identificazione e
sfruttamento di CVE pubblici (esecuzione di codice remoto non autenticata), analisi dei percorsi di
codice vulnerabili dal sorgente, sicurezza JWT (algorithm confusion e il difetto alg=none), forgiatura
di token di autenticazione.

**Sicurezza dei container e Kubernetes**: enumerazione di un pod compromesso, analisi dei permessi del
service account, abuso del permesso nodes/proxy per raggiungere il kubelet, esecuzione di comandi in un
pod privilegiato che monta il filesystem dell'host per l'evasione da container a host.

---

## Contatti

Giampiero Saponaro, junior cybersecurity specialist

- LinkedIn: [linkedin.com/in/giampiero-saponaro-cybersecurity](https://www.linkedin.com/in/giampiero-saponaro-cybersecurity)
- Portfolio: [giampierosap.github.io/GiampieroSaponaro](https://giampierosap.github.io/GiampieroSaponaro)

---

*I report riguardano esclusivamente ambienti di laboratorio autorizzati e challenge CTF concluse.*

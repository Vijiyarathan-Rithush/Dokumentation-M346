# 1. Sie können Vor- und Nachteile der Cloud erläutern

| Vorteile             | Nachteile                  |
| -------------------- | -------------------------- |
| Skalierbarkeit       | Datenschutz und Sicherheit |
| Wartung und Updates  | Anbieterabhängigkeit       |
| Einfaches einrichten | Abhängikeit von Internet   |

---
# 2. Cloud Maturity Model erkläutern

### Klassisch
- Anwendungen werden auf dem physischen Server betrieben
- IT und Entwicklungen arbeiten isoliert voneinander

### Virtualisiert
- Anwendungen werden als virtualisierte Workloads betrieben
- Resesourcen werden effizient verwaltet

### Cloud Ready
- Anwendungen werden per Lift and-Shift in die Cloud verschoben (VM's, DevOps)
- Mehr VM's als Container
- DevOps - Ansätze

### Cloud Native
- Anwendungen werden speziell für Cloud entwickelt ( Cloud-Services, Microservices)
- DevOps / Agil
- Hybrid- / Multicloud

---

# 3. Unterschiede vs Cloud

| Virtualisierung                                                              | Cloud                                                                                             |
| ---------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| Technologie                                                                  | Modell                                                                                            |
| Ermöglicht meherere VM's auf einer einzigen Physischen Hardware zu betreiben | Nutzt Virtualisierung um Rechenleistung, Speicher und Netzwerke über das Internet bereitzustellen |

---
# 4. Vor-  und Nachteile der Virutalisierung
| Vorteile        | Nachteile          |
| --------------- | ------------------ |
| Partitionierung | Lizenzierung       |
| Isolation       | Höhere Komplexität |

---
# 5. Hypervisor erkläutern und Produktbeispiele

Hypervisor ist eine Software mit der die VM's verwaltet und die Hardware-Ressourcen des Hosts auf die vorhandenen VM's verteilt werden.

HyperVisor Typ 1 (Direkt auf Hardware)
- Hyper-V
- QEMU
- ESX

HyperVisor Typ 2 (Auf OS drauf)
- Viruatlbox
- VMware

---
# 6. Prinzip von Public- Private Key Authentifiezierung

Der Benutzer authentifiziert sich, indem er seinen privaten Schlüssel verwendet während der Server den öffentlichen Schlüssel zur Überpprüfung verwendet.



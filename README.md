<p align="center">
  <img src="./assets/banner.png" width="100%" alt="Taje Dine Sidi Mohamed — Étudiant Ingénieur Cloud & Réseaux @ Université de Rennes"/>
</p>

<h3 align="center">👋 Taje Dine Sidi Mohamed — <i>TIJO</i></h3>

<p align="center">
  <img src="https://img.shields.io/badge/Recherche-Stage_Cloud_%C2%B7_DevOps_%C2%B7_R%C3%A9seaux-2EA043?style=for-the-badge" alt="Recherche de stage Cloud, DevOps, Réseaux"/>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/TON-PROFIL/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="mailto:ton.email@exemple.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
  </a>
  <a href="https://TON-PORTFOLIO.com">
    <img src="https://img.shields.io/badge/Portfolio-161B22?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"/>
  </a>
  <img src="https://img.shields.io/badge/Rennes,_France-161B22?style=for-the-badge&logo=googlemaps&logoColor=white" alt="Rennes, France"/>
</p>

---

## 🖥️ Statut système

```console
$ systemctl status tijo.service
● tijo.service - Taje Dine Sidi Mohamed · Cloud & Network Engineering Student
     Loaded: loaded (/etc/universite-de-rennes/cloud-reseaux.conf; enabled)
     Active: active (running) — disponible pour un stage
   Main PID: 2026 (curiosity)
      Tasks: Cloud · DevOps · Réseaux · Observabilité
     Memory: Linux, Docker, Kubernetes, Nginx, Kafka, Wireshark
     CGroup: /formation/ingenieur-cloud-reseaux
             ├─ microservices-ha.service          ● running
             ├─ network-lab.service               ● running
             ├─ elk-monitoring.service            ● starting
             └─ stage.target                      ● waiting for offers

$ journalctl -u tijo.service --no-pager | tail -4
[INFO]  Objectif : concevoir des infrastructures de bout en bout, du câble au cloud
[INFO]  Approche : automatiser, versionner, superviser
[INFO]  Langues  : Français · Arabe · Anglais
[OK]    Prêt à rejoindre une équipe Cloud / DevOps / Réseau en stage
```

---

## 🎬 Comment ça marche — Architectures en action

<p align="center">
  <img src="./assets/architectures.svg" width="100%" alt="Animation : microservices, load balancer, DHCP, DNS, VLAN, TLS, AWS VPC, ELK, Kafka et MapReduce expliqués étape par étape"/>
</p>

---

## 🛠️ Compétences techniques

### ☁️ Cloud, Conteneurs & Orchestration

<p align="left">
  <img src="https://skillicons.dev/icons?i=aws,docker,kubernetes,nginx&theme=dark" alt="AWS, Docker, Kubernetes, Nginx"/>
</p>

### 🌐 Réseaux, Systèmes & Protocoles

<p align="left">
  <img src="https://skillicons.dev/icons?i=linux,git,github,gitlab,vscode&theme=dark" alt="Linux, Git, GitHub, GitLab, VS Code"/>
</p>

<p align="left">
  <img src="https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white" alt="Wireshark"/>
  <img src="https://img.shields.io/badge/VLAN-1F6FEB?style=flat-square&logo=cisco&logoColor=white" alt="VLAN"/>
  <img src="https://img.shields.io/badge/DNS-6E40C9?style=flat-square" alt="DNS"/>
  <img src="https://img.shields.io/badge/DHCP-6E40C9?style=flat-square" alt="DHCP"/>
  <img src="https://img.shields.io/badge/OSPF-1F6FEB?style=flat-square" alt="OSPF"/>
  <img src="https://img.shields.io/badge/TLS%2FSSL-2EA043?style=flat-square" alt="TLS/SSL"/>
  <img src="https://img.shields.io/badge/TCP%2FIP_%C2%B7_IPv4_%C2%B7_IPv6-30363D?style=flat-square" alt="TCP/IP, IPv4, IPv6"/>
</p>

### ⚡ Data Streaming & Code

<p align="left">
  <img src="https://skillicons.dev/icons?i=kafka,python,bash&theme=dark" alt="Kafka, Python, Bash"/>
</p>

<p align="left">
  <img src="https://img.shields.io/badge/MapReduce-66CCFF?style=flat-square&logo=apachehadoop&logoColor=black" alt="MapReduce"/>
</p>

### 📈 Observabilité — Stack ELK

<p align="left">
  <img src="https://img.shields.io/badge/Elasticsearch-005571?style=for-the-badge&logo=elasticsearch&logoColor=white" alt="Elasticsearch"/>
  <img src="https://img.shields.io/badge/Logstash-005571?style=for-the-badge&logo=logstash&logoColor=white" alt="Logstash"/>
  <img src="https://img.shields.io/badge/Kibana-005571?style=for-the-badge&logo=kibana&logoColor=white" alt="Kibana"/>
</p>

### 🌱 En cours d'apprentissage

<p align="left">
  <img src="https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white" alt="Terraform"/>
  <img src="https://img.shields.io/badge/Ansible-EE0000?style=for-the-badge&logo=ansible&logoColor=white" alt="Ansible"/>
  <img src="https://img.shields.io/badge/BGP-1F6FEB?style=for-the-badge" alt="BGP"/>
</p>

> Appris en construisant les projets ci-dessous.

---

## 🏗️ Vision : une infrastructure de bout en bout

```mermaid
flowchart LR
    U["👤 Utilisateurs"] --> DNS["DNS"]
    DNS --> LB["Nginx<br/>Load Balancer (TLS)"]
    LB --> S1["Microservice A"]
    LB --> S2["Microservice B"]
    LB --> S3["Microservice C"]
    S1 & S2 & S3 --> K["Apache Kafka<br/>Streaming"]
    K --> P["Traitement<br/>Python / MapReduce"]
    S1 & S2 & S3 -. logs .-> E["Stack ELK<br/>Supervision"]

    subgraph AWS["☁️ AWS VPC"]
        LB
        S1
        S2
        S3
        K
        P
        E
    end
```

---

## 🚀 Projets phares — Hybride Cloud & Réseaux

| Projet | Description | Stack | Statut |
|:--|:--|:--|:--:|
| 🔀 **[Microservices High-Availability Cluster](https://github.com/tajedinesidimohamed/microservices-ha-cluster)** | Architecture microservices derrière un load balancer avec tolérance aux pannes : un serveur tombe, le trafic bascule automatiquement. | Docker · Nginx · HAProxy · Linux | 🛠️ En cours |
| 📈 **[ELK Log Monitoring](https://github.com/tajedinesidimohamed/elk-log-monitoring)** | Centralisation des logs de serveurs et d'équipements réseau, détection d'anomalies et dashboards Kibana. | Elasticsearch · Logstash · Kibana · Docker | 🛠️ En cours |
| 🌐 **[Enterprise Network Automation Lab](https://github.com/tajedinesidimohamed/network-automation-lab)** | Réseau d'entreprise segmenté (VLANs, DNS, DHCP, OSPF puis BGP), configuré par Ansible et validé par scripts de tests. | Ansible · Python · Linux · Wireshark | 🛠️ En cours |
| ☁️ **[Cloud Multi-Tier Infra (AWS)](https://github.com/tajedinesidimohamed/aws-multi-tier-terraform)** | Infra VPC sécurisée provisionnée par code : subnets publics/privés, tables de routage, passerelles NAT. | Terraform · AWS · VPC | 🛠️ En cours |
| ⚡ **[Realtime Kafka Streaming Pipeline](https://github.com/tajedinesidimohamed/kafka-streaming-pipeline)** | Pipeline distribué de flux de données en temps réel entre plusieurs nœuds serveurs, avec traitement des données. | Kafka · MapReduce · Python · Docker | 🛠️ En cours |

> 💡 Chaque projet est documenté avec un schéma d'architecture, les étapes de déploiement et des captures de démonstration.

---

## 📊 Statistiques GitHub

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=tajedinesidimohamed&show_icons=true&theme=github_dark&hide_border=true&include_all_commits=true" alt="Statistiques GitHub"/>
  <img height="170" src="https://streak-stats.demolab.com?user=tajedinesidimohamed&theme=github-dark-blue&hide_border=true" alt="Série de contributions"/>
</p>

<p align="center">
  <img width="100%" src="https://github-readme-activity-graph.vercel.app/graph?username=tajedinesidimohamed&theme=github-compact&hide_border=true&area=true" alt="Graphique d'activité"/>
</p>

<!-- Serpent de contributions : nécessite le fichier .github/workflows/snake.yml -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/tajedinesidimohamed/tajedinesidimohamed/output/github-snake-dark.svg"/>
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/tajedinesidimohamed/tajedinesidimohamed/output/github-snake.svg"/>
    <img alt="Animation des contributions" src="https://raw.githubusercontent.com/tajedinesidimohamed/tajedinesidimohamed/output/github-snake-dark.svg"/>
  </picture>
</p>

---

<p align="center">
  <i>« Automatiser, versionner, superviser : du câble au cloud. »</i>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=tajedinesidimohamed&color=2EA043&style=flat-square&label=Visites+du+profil" alt="Visites du profil"/>
</p>

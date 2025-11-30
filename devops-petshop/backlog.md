# 🧪 Backlog – Projeto DevOps Petshop (Homelab)

Este backlog organiza as atividades para implementação do pipeline completo da aplicação Petshop no ambiente **homelab**, integrando CI/CD, análise de código, containerização e deploy em Kubernetes.

---

## 🔷 1. Preparação do Repositório

| ID | Atividade | Status |
|----|-----------|--------|
| T1 | Criar repositório `homelab` no GitHub | 🆗 |
| T2 | Criar estrutura de pastas conforme proposta | 🆗 |
| T3 | Adicionar README.md inicial no repositório | 🆗 |
| T4 | Criar diretório `devops-petshop/` | 🆗 |
| T5 | Criar este arquivo `backlog.md` | 🆗 |

---

## 🔷 2. Ambiente Jenkins

| ID | Atividade | Status |
|----|-----------|--------|
| T6 | Criar VM dedicada para CI (Jenkins) | 🆗 |
| T7 | Instalar **Java 17** | 🔲 |
| T8 | Instalar **Jenkins LTS** | 🔲 |
| T9 | Instalar **Docker Engine** e liberar acesso ao Jenkins | 🔲 |
| T10 | Instalar **Trivy** para análise de vulnerabilidades | 🔲 |
| T11 | Instalar **kubectl** e validar acesso ao cluster | 🔲 |
| T12 | Instalar **Ansible** (para evoluir na etapa futura) | 🔲 |
| T13 | Validar comunicação com o cluster (`kubectl get nodes`) | 🔲 |

---

## 🔷 3. Configuração de Ferramentas externas

| ID | Atividade | Status |
|----|-----------|--------|
| T14 | Subir **SonarQube (Docker container)** | 🔲 |
| T15 | Criar token no Sonar e armazenar no Jenkins | 🔲 |
| T16 | Instalar plugin Sonar no Jenkins | 🔲 |
| T17 | Instalar plugin OWASP Dependency Check | 🔲 |
| T18 | Instalar plugins Docker (Pipeline, API etc.) | 🔲 |
| T19 | Instalar plugins Kubernetes + Maven | 🔲 |
| T20 | Configurar tools no Jenkins (`jdk17`, `maven3`, `sonar-scanner`) | 🔲 |

---

## 🔷 4. Git e Código da Aplicação

| ID | Atividade | Status |
|----|-----------|--------|
| T21 | Criar fork do repositório da aplicação Petshop | 🔲 |
| T22 | Clonar projeto localmente e adaptar conforme necessário | 🔲 |
| T23 | Adicionar Dockerfile no projeto | 🔲 |
| T24 | Criar pasta `k8s/` com manifests (deployment/service) | 🔲 |

---

## 🔷 5. Pipeline Jenkins (Jenkinsfile)

| ID | Atividade | Status |
|----|-----------|--------|
| T25 | Stage 1 – Clean workspace | 🔲 |
| T26 | Stage 2 – Checkout SCM | 🔲 |
| T27 | Stage 3 – Maven Compile & Unit Tests | 🔲 |
| T28 | Stage 4 – SonarQube Analysis | 🔲 |
| T29 | Stage 5 – OWASP Dependency Check | 🔲 |
| T30 | Stage 6 – Build & Push Docker Image | 🔲 |
| T31 | Stage 7 – Deploy no Kubernetes | 🔲 |
| T32 | Implementar notificações (futuro - opcional) | 🔲 |

---

## 🔷 6. Kubernetes Deployment

| ID | Atividade | Status |
|----|-----------|--------|
| T33 | Criar namespace `petshop` | 🔲 |
| T34 | Criar deployment usando imagem docker | 🔲 |
| T35 | Criar service (NodePort ou LoadBalancer) | 🔲 |
| T36 | Validar acesso via browser (http://NODE:PORT/jpetstore) | 🔲 |

---

## 🔷 7. Evolução e Melhoria Contínua

| ID | Atividade | Status |
|----|-----------|--------|
| T37 | Implementar scanning de imagem com Trivy no pipeline | 🔲 |
| T38 | Adicionar etapa de segurança com SAST | 🔲 |
| T39 | Adicionar teste automático de deploy | 🔲 |
| T40 | Gerar documentação de arquitetura (`docs/arquitetura.md`) | 🔲 |
| T41 | Preparar post para Medium com processo do projeto | 🔲 |
| T42 | Integrar monitoramento (Prometheus/Grafana) | 🔲 |
| T43 | Considerar uso de Helm Charts (evolução) | 🔲 |
| T44 | Considerar GitOps (com ArgoCD ou FluxCD) | 🔲 |

---

## 🏁 Finalização (fase inicial do projeto)

| ID | Atividade | Status |
|----|-----------|--------|
| T45 | Pipeline rodando com sucesso (CI + Docker + Deploy K8s) | 🔲 |
| T46 | Documentação básica publicada | 🔲 |
| T47 | Commitar projeto completo no `homelab` | 🔲 |
| T48 | Validar acesso externo da aplicação | 🔲 |

---

## 👤 Autor

Feito por **Joás Pardim Araújo**  
*Arquiteto de Soluções | DevOps | Homelab & Cloud Enthusiast* 🚀


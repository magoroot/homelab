# 🎯 SonarQube – Recurso do Homelab

Este diretório contém a configuração do **SonarQube** utilizada no homelab, com banco de dados PostgreSQL externo em um LXC (`172.16.30.16`).

## 📁 Estrutura

- `docker-compose.yml` – Orquestração do container do SonarQube
- `.env` – Configuração (imagem, credenciais, host do banco, porta)
- `sonarqube/` – Dados, logs e extensões do SonarQube (persistência)

## 🗄️ Banco de Dados

- Servidor PostgreSQL: `172.16.30.16:5432`
- Banco: `sonarqube`
- Usuário: `sonar`

A criação do banco/usuário é feita diretamente no LXC do PostgreSQL (fora do Docker).

## 🚀 Como subir

```bash
cd homelab/recursos/sonarqube

mkdir -p sonarqube/data sonarqube/logs sonarqube/extensions

docker compose up -d
docker ps

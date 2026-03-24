# 🔐 AccessPIM — Controle de Acesso por Área

Sistema web para registro, monitoramento e auditoria de acessos a áreas restritas em ambientes industriais.

## 📌 Visão Geral

O **AccessPIM** foi desenvolvido para resolver um problema comum no Polo Industrial de Manaus: o controle manual e pouco confiável de entrada e saída em áreas críticas.

O sistema substitui processos baseados em papel e planilhas por uma solução digital com:

* Registro em tempo real
* Histórico auditável
* Dashboard com indicadores operacionais
* Controle de acessos autorizados e negados

## 🎯 Objetivo

Garantir rastreabilidade, segurança e visibilidade sobre o fluxo de pessoas em áreas restritas, permitindo tomada de decisão rápida por gestores.

## 👥 Perfis de Usuário

* **Operador de Segurança**

  * Registra entradas e saídas
  * Uso contínuo no dia a dia

* **Gestor**

  * Monitora dashboard
  * Audita acessos

* **Administrador**

  * Gerencia colaboradores e áreas

## 🧱 Arquitetura

* **Frontend:** Angular 21 + Tailwind CSS
* **Backend:** Node.js + Express
* **Banco de Dados:** PostgreSQL
* **Autenticação:** JWT

## 🗄️ Modelagem de Dados

Principais entidades:

* **Colaborador**
* **Área**
* **Registro de Acesso**

Cada acesso registra:

* Quem acessou
* Qual área
* Tipo (entrada/saída)
* Status (autorizado/negado)
* Timestamp
* Operador responsável

## 📊 Funcionalidades

### 🔐 Autenticação

* Login com JWT
* Rotas protegidas

### 👤 Colaboradores

* CRUD completo
* Ativação/Desativação

### 🏭 Áreas

* Cadastro com nível de risco
* Definição de capacidade máxima

### 📋 Registro de Acesso

* Entrada e saída manual
* Registro de acessos negados com justificativa

### 📈 Dashboard

* Total de acessos do dia
* Acessos negados
* Ocupação atual
* Área com maior movimentação

### 📜 Histórico

* Filtros por:

  * Período
  * Área
  * Colaborador

## ⚙️ Requisitos Técnicos

* JWT para autenticação
* Hash de senha com bcrypt
* API REST protegida
* Variáveis sensíveis em `.env`

## 🚧 Roadmap (Evoluções Futuras)

* Autorização automática por cargo
* Exportação CSV
* Mapa de ocupação em tempo real
* Integração com hardware (RFID, biometria)

## 🧪 Status do Projeto

🚀 Em desenvolvimento (MVP)

## 📎 Sobre o Projeto

Projeto desenvolvido como parte da formação Full Stack do INDT, com foco em resolver problemas reais da indústria utilizando tecnologias modernas.

---

💡 *Este projeto demonstra habilidades em desenvolvimento full stack, modelagem de dados, autenticação segura e construção de sistemas voltados para operações reais.*

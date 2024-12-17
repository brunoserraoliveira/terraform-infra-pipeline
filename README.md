# 🚀 CI/CD Pipeline com Terraform, AWS e GitHub Actions

Este repositório implementa uma **Pipeline CI/CD** que provisiona infraestrutura na AWS utilizando **Terraform** e **GitHub Actions**. A infraestrutura possui dois ambientes: **DEV** e **PROD**, com validação e provisionamento automático ao realizar um **push** no repositório.

---

## 📋 Funcionalidades

1. **Ambientes DEV e PROD**:
   - A pipeline executa os comandos do Terraform para criar ou destruir a infraestrutura em ambos os ambientes.
   - **DEV** é utilizado para validação e testes.
   - **PROD** é utilizado para produção.

2. **Execução Automática**:
   - Ao fazer **push** para o repositório, a pipeline é acionada automaticamente.
   - **Terraform** executa as seguintes etapas:
     - `terraform validate`
     - `terraform init`
     - `terraform plan`
     - `terraform apply`

3. **Destruir Infraestrutura**:
   - Existe um controle em um arquivo **JSON** que permite escolher se a infraestrutura deve ser destruída.
   - Defina a opção **destroy** como:
     - `true`: A infraestrutura será destruída.
     - `false`: A infraestrutura permanecerá intacta.

---

## 🛠️ Tecnologias Utilizadas

- **Terraform**: Gerenciamento de infraestrutura como código.
- **AWS**: Provedor de infraestrutura.
- **GitHub Actions**: Automação de CI/CD.
- **JSON**: Configuração para controle de destruição da infraestrutura.

---

## 🎓 Créditos

Projeto desenvolvido com base na aula do **Professor Bruno Garcia**.  
Assista à aula completa no YouTube: [CI/CD com Terraform e GitHub Actions](https://www.youtube.com/watch?v=1TNAUW7_bC0&list=PLxCh3SsamNs56-Jq8_UsnShGYiRexXkdY&index=1).

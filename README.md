
# Fase 1 — DevOps na Prática (Starter Kit)

Este repositório contém um projeto mínimo para você cumprir a **Fase 1 (Configuração e Automação Inicial)**:

- ✅ **Documento de Planejamento** (`docs/plano-projeto.md`)
- ✅ **Pipeline de Integração Contínua** com **GitHub Actions** (`.github/workflows/ci.yml`)
- ✅ **Aplicação de exemplo** em Node.js com **testes automatizados** (Jest)
- ✅ **Scripts de IaC** em **Terraform** (provisionamento de uma instância EC2 simples)

> **Como usar**
>
> 1. Crie um repositório no GitHub e suba todos os arquivos deste pacote.
> 2. Verifique a aba **Actions**: o workflow será executado automaticamente.
> 3. Abra e edite `docs/plano-projeto.md` com as informações do seu projeto e o link do repositório.
> 4. (Opcional) Configure suas credenciais AWS localmente para testar o Terraform: `terraform init`, `terraform fmt -check`, `terraform validate`, `terraform plan`.

---

## Scripts úteis (Node.js)
```bash
cd app
npm ci
npm test
npm start  # (se você criar um server http depois)
```

## Terraform (opcional)
```bash
cd terraform
cp terraform.tfvars.example terraform.tfvars
terraform init
terraform fmt -check
terraform validate
terraform plan
# terraform apply  # apenas se você desejar criar a infra de verdade
```

> **Atenção:** para `apply`, você precisa de uma conta AWS, credenciais válidas e eventuais custos podem ser gerados.

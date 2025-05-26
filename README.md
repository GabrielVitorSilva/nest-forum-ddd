# 🚀 Nest Forum DDD

Um fórum moderno construído com NestJS, seguindo os princípios do Domain-Driven Design (DDD) e Clean Architecture.

## ✨ Tecnologias e Padrões

### 🛠️ Stack Principal
- **NestJS** - Framework Node.js para construção de aplicações escaláveis
- **TypeScript** - Superset JavaScript com tipagem estática
- **Prisma** - ORM moderno para TypeScript/Node.js
- **PostgreSQL** - Banco de dados relacional
- **Redis** - Cache e gerenciamento de sessões
- **AWS S3 / Cloudfare R2** - Armazenamento de arquivos
- **JWT** - Autenticação e autorização
- **Zod** - Validação de dados em tempo de execução

### 🏗️ Padrões de Arquitetura
- **Domain-Driven Design (DDD)** - Organização do código baseada no domínio do negócio
- **Clean Architecture** - Separação clara de responsabilidades
- **SOLID Principles** - Princípios de design orientado a objetos
- **Repository Pattern** - Abstração da camada de persistência
- **Factory Pattern** - Criação de objetos complexos
- **Strategy Pattern** - Implementação de diferentes estratégias de upload
- **Dependency Injection** - Injeção de dependências para melhor testabilidade

## 🚀 Como Executar

### Pré-requisitos
- Node.js 18+
- Docker e Docker Compose
- PNPM (gerenciador de pacotes)

### Configuração do Ambiente

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/nest-forum-ddd.git
cd nest-forum-ddd
```

2. Instale as dependências:
```bash
pnpm install
```

3. Configure as variáveis de ambiente:
```bash
cp .env.example .env
```

4. Inicie os containers Docker:
```bash
docker-compose up -d
```

5. Execute as migrações do Prisma:
```bash
pnpm prisma migrate dev
```

6. Inicie a aplicação em modo desenvolvimento:
```bash
pnpm start:dev
```

## 🧪 Testes

O projeto utiliza Vitest para testes unitários e e2e:

```bash
# Testes unitários
pnpm test

# Testes com watch mode
pnpm test:watch

# Testes e2e
pnpm test:e2e

# Cobertura de testes
pnpm test:cov
```

## 📚 Documentação da API

A documentação da API está disponível através do Swagger UI quando a aplicação estiver rodando:

```
http://localhost:3000/api
```

## 🏗️ Estrutura do Projeto

```
src/
├── domain/           # Entidades e regras de negócio
├── application/      # Casos de uso e serviços
├── infrastructure/   # Implementações concretas (repositories, etc)
└── presentation/     # Controllers e DTOs
```

## 🔒 Segurança

- Autenticação JWT
- Validação de dados com Zod
- Proteção contra ataques comuns
- Variáveis de ambiente seguras

## 🤝 Contribuindo

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👥 Autor

- Seu Nome - [@Gabriel Vitor](https://github.com/GabrielVitorSilva)


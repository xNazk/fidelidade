# Vulcanus Grill — Sistema de Fidelidade

## Estrutura do projeto

```
vulcanus-fidelidade/
├── index.html        ← sistema completo
├── public/
│   └── logo.png      ← logo do Vulcanus Grill
├── vercel.json       ← configuração da Vercel
└── README.md
```

## Como fazer o deploy na Vercel

### Opção 1 — Via interface web (mais simples)

1. Acesse [vercel.com](https://vercel.com) e faça login
2. Clique em **"Add New Project"**
3. Escolha **"Deploy without a Git repository"**
4. Arraste a pasta `vulcanus-fidelidade` inteira para a área de upload
5. Clique em **Deploy**
6. Pronto! A Vercel vai gerar uma URL do tipo `vulcanus-fidelidade.vercel.app`

### Opção 2 — Via GitHub (recomendado para futuras atualizações)

1. Crie um repositório no GitHub e suba esta pasta
2. Na Vercel, clique em **"Add New Project"** → **"Import Git Repository"**
3. Selecione o repositório criado
4. Clique em **Deploy**
5. A cada push no GitHub, o site atualiza automaticamente

---

## Senha do atendente

```
Admin@Grill2602
```

Guarde essa senha com segurança. Para alterá-la, edite a linha abaixo em `index.html`:

```js
const ADMIN_PASS = "Admin@Grill2602";
```

---

## Dados dos clientes

Os dados ficam salvos no `localStorage` do navegador de cada dispositivo.
Isso significa que funciona sem banco de dados externo, mas **os dados são locais** — 
se o atendente usar um dispositivo diferente, não verá os clientes cadastrados no outro.

**Solução futura:** Para centralizar os dados, será necessário adicionar um banco de dados
(Supabase ou similar). Avise quando quiser dar esse próximo passo.

---

## Funcionalidades

- ✅ Cadastro de cliente com nome, CPF e WhatsApp
- ✅ Consulta do cartão por CPF
- ✅ Visualização dos carimbos (10 por ciclo)
- ✅ Painel do atendente com senha
- ✅ Registro de pedidos
- ✅ Resgate automático do combo ao completar 10 pedidos
- ✅ Histórico de resgates por cliente
- ✅ Busca por nome ou CPF
- ✅ Funciona em celular (layout responsivo)
- ✅ Suporte a modo escuro automático
- 

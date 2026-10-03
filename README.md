# JogosEnsino

MVP da plataforma de jogos de estudo baseada no PRD.

## Stack
Next.js + TypeScript + Supabase Auth/PostgreSQL + Vercel.

## Configuração
1. Execute `supabase/schema.sql` no SQL Editor do Supabase.
2. Copie `.env.example` para `.env.local`.
3. Preencha as variáveis do Supabase e `OPENAI_API_KEY`.
4. Rode `npm install` e `npm run dev`.
5. Para Vercel, configure as mesmas variáveis no projeto.

A chave da IA fica somente no servidor e o RLS limita os dados ao usuário autenticado.

## Fluxo
Login → adicionar matéria → extrair PDF/DOCX/TXT ou texto → gerar estrutura e perguntas → salvar → jogar → registrar tentativas → voltar pela biblioteca.

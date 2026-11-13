# O Segredo dos Brigadeiros Perfeitos — funil
Site estático (sem build). Edite `config.js`. No Vercel: importar o repositório, Framework "Other", Deploy.
Ver instruções de Supabase (presença e compras) abaixo.
## Supabase
Preencher SUPABASE_URL e SUPABASE_ANON_KEY (chave pública). Realtime Presence/Broadcast funcionam sem tabelas.
## Compras reais
O webhook do checkout deve ser recebido por um servidor (ex.: função Vercel) que faz broadcast no canal `vsl-viewers`, evento `purchase`, com `{name}`. Nunca expor a service_role no frontend.

# RŌGUE. Prospect — MVP 1.0

Ferramenta interna de prospeção comercial, auditoria visual e CRM para PMEs, inicialmente focada em Ponta Delgada.

## Publicar no GitHub Pages (repositório público)

1. Cria um repositório público chamado `rogue-prospect`.
2. Carrega **os ficheiros desta pasta para a raiz** do repositório (`index.html`, `app.js`, `styles.css`, `manifest.webmanifest`, `icon.svg`). Não carregues apenas o ZIP.
3. Vai a **Settings → Pages → Build and deployment**.
4. Em **Source**, escolhe **Deploy from a branch**; seleciona **main** e **/(root)**; guarda.
5. O endereço deverá ser `https://TEU-UTILIZADOR.github.io/rogue-prospect/` após a publicação.

## O que funciona

- Dashboard e lista de empresas com filtros
- Registo e edição de empresas, websites, redes sociais, notas e próximos passos
- Pesquisa assistida via Google Maps (abre no navegador; sem importação automática)
- Auditoria manual com quatro critérios de 0 a 5 e evidências
- Score de qualidade visual e score indicativo de oportunidade
- Histórico de atividades e pipeline comercial
- Relatório interno imprimível em PDF pelo navegador
- Exportação CSV, backup JSON e restauro JSON
- Interface responsiva e manifesto para instalação como webapp

## Limitações importantes

**Esta versão é 100% estática e local.** Os dados são guardados em `localStorage` no dispositivo e navegador em que são introduzidos. Não há sincronização entre PC e Android, autenticação, Supabase, análise de imagem por IA, recolha automática de empresas ou envio de emails. Limpar os dados do navegador pode apagar o CRM. Exporta regularmente o backup JSON.

**Repositório público:** todo o código é público, mas os dados locais do teu navegador não são publicados no GitHub. Não introduzas chaves secretas no código. Para guardar contactos pessoais e informação comercial sensível, a próxima fase deve implementar autenticação, regras de acesso e base de dados privada.

## Próxima fase

Migrar para React + Tailwind e Supabase com autenticação, armazenamento privado e integração autorizada de pesquisa de negócios. A versão atual evita dependências externas e funciona diretamente no GitHub Pages.

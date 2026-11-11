# Viver em Paz para Morrer em Paz — Quintino Ferreira da Silva

Página estática em português brasileiro para apresentar a obra *Viver em Paz para Morrer em Paz*, de Mario Sergio Cortella, e encaminhar o visitante à oferta oficial na Hotmart.

## Estrutura

- `site/index.html`: página principal, metadados e conteúdo.
- `site/style.css`: identidade visual e layout responsivo.
- `site/script.js`: menu móvel, ano do rodapé e configuração do CTA.
- `site/assets/`: capa e imagem de divulgação.
- `site/favicon.svg`: ícone do site.
- `hotmart-copy.md`: texto de apoio para cadastro da oferta.
- `assets/source/`: material-fonte mantido fora da pasta pública.

## Publicação na Vercel

O projeto é estático: não usa backend, `package.json`, `pnpm-lock.yaml` nem etapa de compilação.

A configuração versionada em `vercel.json` informa à Vercel que os arquivos públicos estão em `site/`. No painel do projeto, mantenha:

- **Root Directory:** `./` (raiz do repositório).
- **Framework Preset:** Other.
- **Build Command:** vazio / desativado.
- **Install Command:** vazio / desativado.
- **Output Directory:** definido por `vercel.json` como `site`.

Depois de conectar o repositório, publique a branch `main`. Não é necessário criar um workflow do GitHub Actions para a publicação padrão pela integração Git da Vercel.

## Checkout

O botão de compra direciona para o checkout informado pelo responsável pela oferta:

`https://pay.hotmart.com/U108118072R`

O link é configurado em `HOTMART_CHECKOUT_URL`, no início de `site/script.js`, e abre uma página de pagamento.

## Conteúdo e uso

- A área de depoimentos contém apenas espaços reservados; publique avaliações somente quando forem reais e autorizadas.
- O selo “Leitura para refletir” é um elemento visual, não uma certificação ou garantia.
- O PDF-fonte não faz parte da pasta pública. Sua distribuição depende da licença e das autorizações aplicáveis.
- Confirme na Hotmart as condições comerciais, o acesso e as políticas vigentes antes de divulgar a oferta.

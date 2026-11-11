# Apresentação JRS/HNRe — Inspeções de Saúde no Serviço Militar Temporário

Site estático pronto para publicar no **GitHub Pages**. Não há build: basta subir esta pasta como está.

## Conteúdo

| Arquivo | Função |
|---|---|
| `index.html` | Apresentação completa (33 slides), autocontida — fontes, imagens e scripts embutidos. Sem barra de miniaturas. |
| `og-capa.png` | Imagem de pré-visualização (Open Graph / Twitter), 1200×630. |
| `docs/` | Pasta para os PDFs baixados pelos botões de download dos slides de referência. |
| `.nojekyll` | Desativa o Jekyll no GitHub Pages (serve os arquivos como estão). |

## Tarefas para o Claude Code

1. Criar o repositório (ex.: `apresentacao-jrs`) e enviar **todo o conteúdo desta pasta** para a raiz do branch `main`.
2. Ativar o GitHub Pages: *Settings → Pages → Deploy from a branch → main / (root)*.
3. **Ajustar a URL absoluta da imagem de pré-visualização.** No `<head>` do `index.html`, trocar o valor `og-capa.png` (exatamente duas ocorrências: `og:image` e `twitter:image`) por:
   `https://<USUARIO>.github.io/<REPO>/og-capa.png`
   e acrescentar `<meta property="og:url" content="https://<USUARIO>.github.io/<REPO>/">`.
   Redes sociais (WhatsApp, LinkedIn, Facebook) exigem URL absoluta.
   O `index.html` é grande (~9 MB, imagens em base64): editar **apenas** essas linhas do `<head>`, com substituição de texto — não reformatar o arquivo.
4. Colocar os PDFs em `docs/` com **estes nomes exatos** (os botões já apontam para eles):
   - `docs/DGPM-406-Cap11.pdf` — DGPM-406, 9ª Rev., Capítulo 11
   - `docs/NORDINAVNATAL-90-03.pdf` — NORDINAVNATAL nº 90-03, de 28/09/2026
   - `docs/Lei-4375-1964-LSM.pdf` — Lei nº 4.375/1964 (Lei do Serviço Militar)
5. Testar: abrir a URL publicada, avançar com → / clique, e validar a pré-visualização em https://www.opengraph.xyz/ ou no WhatsApp.

## Atenção

- Repositório público ⇒ os PDFs em `docs/` ficam públicos. Confirmar a classificação de cada documento antes de publicar.
- Não editar o conteúdo dos slides no `index.html`: ele é gerado. Alterações de conteúdo devem ser feitas no projeto de origem e o arquivo regenerado.

## Uso da apresentação

- → / clique / espaço: avança (inclui os passos internos dos fluxogramas e dos slides com clique).
- ←: volta.
- Slide 1: a fachada noturna fica parada até o primeiro clique, que dispara a abertura (~16 s).
- F: tela cheia (atalho do navegador/apresentação).

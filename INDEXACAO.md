# Indexação no Google

## Publicar

As alterações locais precisam ser publicadas nos dois projetos da Vercel.
O biolink tem repositório próprio: publicar o site principal não publica o biolink.
Envie os HTMLs alterados, robots.txt e sitemap.xml de cada projeto; no biolink,
envie também data/site.js.

Depois da publicação, verifique se estes arquivos abrem com HTTP 200:

- https://www.helenaholanda5508.com.br/sitemap.xml
- https://www.helenaholanda5508.com.br/robots.txt
- https://biolink.helenaholanda5508.com.br/sitemap.xml
- https://biolink.helenaholanda5508.com.br/robots.txt

## Google Search Console

1. Abra https://search.google.com/search-console/ com a conta responsável pelo site.
2. Adicione uma propriedade de domínio: helenaholanda5508.com.br.
3. Copie o registro TXT fornecido pelo Google e adicione no provedor de DNS do domínio.
   Essa propriedade cobre tanto www quanto biolink. O valor TXT depende da sua conta.
4. Após verificar a propriedade, em Sitemaps, envie os dois endereços de sitemap acima.
5. Em Inspeção de URL, inspecione cada endereço abaixo, teste o URL publicado
   e clique em Solicitar indexação:
   - https://www.helenaholanda5508.com.br/
   - https://biolink.helenaholanda5508.com.br/
6. Acompanhe o relatório de indexação de páginas e eventuais motivos de exclusão.

O #inicio é uma seção da página inicial, não uma página separada.
As telas com # do biolink também não entram como páginas independentes no sitemap.
Cada domínio tem seu próprio endereço canônico: o biolink não aponta o canônico
para o site principal, pois queremos que os dois possam aparecer na pesquisa.

A ausência de robots.txt não bloqueava o Google por si só. O novo arquivo permite
o rastreamento e informa a localização do sitemap. Esses ajustes ajudam na descoberta,
mas não garantem indexação nem posição na pesquisa. A análise pode levar dias ou semanas.

Referência: https://developers.google.com/search/docs/crawling-indexing/ask-google-to-recrawl?hl=pt-br

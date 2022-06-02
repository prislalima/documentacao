
# Como instalar o Docsify

Existem duas maneiras de instalar o Docsify:

   1. Interface de linha de comando (CLI) do Docsify por meio do NPM
   2. Manualmente escrevendo seu próprio index.html

A Docsify recomenda a abordagem NPM, mas usaremos a segunda opção. 
Se você quiser usar o NPM, siga as instruções no guia de quick-start guide.

# Inicialização manual

Se você não gostar do npm ou tiver problemas para instalar a ferramenta, você pode criar manualmente index.html:

```html
<!-- index.html -->

<!DOCTYPE html>
<html>
  <head>
    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
    <meta name="viewport" content="width=device-width,initial-scale=1" />
    <meta charset="UTF-8" />
    <link
      rel="stylesheet"
      href="//cdn.jsdelivr.net/npm/docsify@4/themes/vue.css"
    />
  </head>
  <body>
    <div id="app"></div>
    <script>
      window.$docsify = {
        //...
      };
    </script>
    <script src="//cdn.jsdelivr.net/npm/docsify@4"></script>
  </body>
</html>
```
### Especificando versões do docsify

?> Observe que em ambos os exemplos abaixo, os URLs docsify precisarão ser atualizados manualmente quando uma nova versão principal do docsify for lançada (e.g. `v4.x.x` => `v5.x.x`). Verifique o site docsify periodicamente para ver se uma nova versão principal foi lançada.

Especificar uma versão principal na URL (`@4`) permitirá que seu site receba melhorias ininterruptas (ou seja, atualizações "menores") e correções de bugs (ou seja, atualizações de "patch") automaticamente. Essa é a maneira recomendada de carregar recursos docsify.

```html
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify@4/themes/vue.css" />
<script src="//cdn.jsdelivr.net/npm/docsify@4"></script>
```

Se você preferir bloquear o docsify para uma versão específica, especifique a versão completa após o símbolo `@` na URL. Essa é a maneira mais segura de garantir que seu site tenha a mesma aparência e comportamento, independentemente de quaisquer alterações feitas em versões futuras do docsify.

```html
<link
  rel="stylesheet"
  href="//cdn.jsdelivr.net/npm/docsify@4.11.4/themes/vue.css"
/>
<script src="//cdn.jsdelivr.net/npm/docsify@4.11.4"></script>
```



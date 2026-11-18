# FS Track Designer

Ferramenta web para desenhar pistas de Formula Student por elementos — retas, curvas com raio e ângulo
exatos, hairpins, slaloms, chicanes — verificando se cabem na área de asfalto, com fluxo Google Earth:

1. Desenhar o polígono da zona de testes no Google Earth → exportar KML → importar aqui
   (ou usar um screenshot georreferenciado como fundo).
2. Construir a pista; a ferramenta verifica área, margens, sobreposições, fecho do circuito e regras de layout.
3. Exportar `.kml` (ou `.geojson`) → importar no Google Earth; `.csv` com a posição de cada cone.

Site estático num único `index.html`: sem servidor, sem build. Projetos ficam no browser (localStorage)
e podem ser guardados/abertos como `.json`.

## Publicar no Netlify
- https://app.netlify.com/drop → arrastar esta pasta.
- Atualizar: no site, separador **Deploys** → arrastar a pasta nova.

Regras de layout (hairpin, retas, slalom) são valores típicos e editáveis — confirmar no regulamento em vigor.

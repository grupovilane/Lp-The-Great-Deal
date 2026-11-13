# Landing page · Nova sala The Great Deal

Página única (`index.html`) para agendar aula teste. Abra no navegador ou suba a pasta inteira (com `assets/`) em qualquer hospedagem.

Direção visual: cópia do design system do template "The Code Company" do Aura (pasta `the-code-company-35.aura.build`):
Tailwind + Inter, títulos em caixa alta, botões retos, foto do topo em pílula com contornos pulsando, faixa azul de destaques
e rodapé azul-marinho com onda, a foto do Ed e colunas de navegação, endereço e contato. Cores da marca: azul-marinho #1B1464 (títulos, faixa de destaques, rodapé) e vermelho #ED1F24 (botões, destaques e o anel da foto do topo, como no logo).

Endereço: R. Manoel da Nóbrega, 1016 - Centro, Diadema - SP (com link para o Google Maps).

Conteúdo baseado na reunião de 9/10/2026 com o Ed: sala nova em Diadema (Grande ABC), Método DR (metodologia criada pelo Ed),
turmas dinâmicas, aulas kids, área de espera, cafezinho com a turma e turmas de janeiro.

## O que ajustar antes de publicar

Procure por `EDITAR` dentro do `index.html`:

1. **WhatsApp**: link do ícone no topo e no rodapé.
2. ~~Fotos do carrossel~~: todas as 12 fotos já são reais.

## Fotos

Em `assets/Fotos/`: `sala.webp` (topo e carrossel), `sala2.webp`, `sala3.jpeg`, `ed-sala.jpeg`, `cafe.jpg` e `turma1` a `turma7.jpeg` (carrossel; originais das novas em `novas/`), `edcarlos.png` (rodapé, sem fundo).
`sala1.png` e `sala2.png` são os originais. Para pôr uma foto nova no carrossel, copie um bloco `<figure class="sala-card ...">` na seção `id="sala"` e troque o `src`.

## Vídeo

Seção "Quantas oportunidades você está deixando passar?", logo depois da faixa azul de destaques.
Arquivos: `assets/video/video-aula-teste.mp4` (720p, H.264, 5 MB, convertido do `originais/IMG_7826.MOV`) e a capa `video-aula-teste-capa.jpg`.
Toca sem som quando aparece na tela (as legendas estão no vídeo); o botão de play grande toca com som.
O vídeo original (150 MB) fica em `originais/`, fora de `assets/`: não precisa subir essa pasta.

## Avaliações do Google

Seção `id="avaliacoes"`, depois da Sala Nova: 10 avaliações reais do Google Meu Negócio (textos como os alunos escreveram, todas de 5 estrelas),
nota 5,0 e 49 avaliações (números do perfil em novembro/2026). O botão "Ver todas no Google" abre o perfil no Maps:
https://www.google.com/maps?cid=2128443191346307554

As avaliações são uma cópia fixa: para atualizar, edite os blocos `<figure class="review-card ...">` e os números "5,0" e "49". O número antigo (715 avaliações do perfil perdido) foi retirado.

## Formulário

Fica na seção `id="aula-teste"`, depois do Método DR, com a foto do Ed ao lado. Todos os botões de agendar (e o "Aplicar o método") levam para ela.

Coleta nome, telefone (com máscara), e-mail e nível de inglês, valida os campos e mostra a tela de confirmação.
Por enquanto **não envia os dados para lugar nenhum**. Para integrar, procure `INTEGRAÇÃO` no fim do arquivo:
o objeto `lead` já sai montado (inclusive com as UTMs da URL), é só fazer o `fetch` para o webhook do CRM.

## Versões

Versões anteriores guardadas para referência:
- `versoes/index-v1-editorial.html`: estilo editorial creme.
- `versoes/index-v2-clean.html`: estilo clean claro com as cores do logo ("English Club").
- `versoes/index-v3-antes-pilula.html`: versão com a foto do topo ainda em círculo.
- `versoes/index-v4-preto-e-branco.html`: versão em preto e branco, antes das cores da marca.
- `versoes/index-v5-antes-carrossel.html`: versão com a grade 2x2 de fotos, antes do carrossel.
- `versoes/index-v6-form-no-topo.html`: versão com o formulário no topo, ao lado da foto da sala.
- `versoes/index-v7-antes-avaliacoes.html`: versão anterior à seção de avaliações do Google.

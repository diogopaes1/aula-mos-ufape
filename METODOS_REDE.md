# Rede de conceitos e variáveis

A análise organiza os textos da turma. Não extrai resultados quantitativos de artigos, avalia a qualidade das fontes ou estabelece relações causais.

## 1. Extração das palavras-chave

O vocabulário técnico identifica expressões completas antes de palavras isoladas e normaliza siglas e sinônimos definidos. Urease, fosfatase, matéria orgânica do solo, carbono orgânico total (COT), carbono da biomassa microbiana (CBM) e respiração basal do solo (RBS) permanecem identificáveis quando mencionados. Fosfatase ácida/alcalina, carbono particulado/POM e carbono associado a minerais/MAOM são conceitos distintos. CO₂ não é convertido automaticamente em respiração.

O léxico derivado de UD Portuguese Bosque 2.16 conserva NOUN/ADJ somente quando representam pelo menos 70% das anotações da forma, calculados sobre **todas** as classes. Não é um etiquetador contextual neural. Candidatos adicionais seguem padrões de substantivo, adjetivos e complemento nominal em português; exigem expressão composta e presença em duas unidades de texto. Suas formas observadas preservam a concordância. Palavras funcionais e substantivos genéricos isolados são filtrados. Citações autor–ano, DOI, URLs, perguntas e a caixa de referências não entram na extração.

Ordenação: `(1 + ln(menções)) × (1 + ln((1 + participantes)/(1 + autores)))`, com fatores 1,3 para expressões compostas e 1,5 para termos técnicos. É uma adaptação explícita de frequência e frequência documental, com prioridade técnica, não o algoritmo PatternRank completo. Todas as variáveis reconhecidas são acrescentadas mesmo além do limite visual escolhido; nenhum termo é criado se não houver menção.

Inspiração para extração por padrões nominais e matrizes de termos: [KeyphraseVectorizers](https://github.com/TimSchopf/KeyphraseVectorizers). Dados e classes gramaticais: [UD em português](https://universaldependencies.org/pt/), [Bosque r2.16](https://github.com/UniversalDependencies/UD_Portuguese-Bosque/tree/r2.16). [Atribuição linguística de Rademaker et al. (2017)](https://aclanthology.org/W17-6523/).

## 2. Rede, comunidades e disposição

Uma aresta reúne dois termos na mesma frase ou linha, com até 200 caracteres entre eles. Seu peso conta unidades de texto distintas; repetições do par na mesma unidade contam uma vez. A área dos nós cresce com o grau entre as arestas **exibidas**, com tamanho mínimo para seleção. Contagens, autores, temas e trechos são conferíveis no inspetor e no JSON.

Disposições: ForceAtlas2, ForceAtlas2 com LinLog, circular e por comunidades. ForceAtlas2 usa a implementação oficial incorporada, seguida por ajuste ao espaço da tela e afastamento dos rótulos; as distâncias visuais não têm escala científica. Movimento em quadros sucessivos, pausa/retomada, arraste, deslocamento da vista e zoom. Preferência do sistema por movimento reduzido é respeitada.

Comunidades: Louvain, fusão gulosa por ganho de modularidade ou componentes conectados. A resolução controla a modularidade nos dois primeiros métodos. Louvain usa `randomWalk: false` para reprodutibilidade; rótulos C1, C2 etc. dependem do recorte. Um componente conectado não equivale necessariamente a uma comunidade temática.

Bibliotecas fixadas: Graphology 0.26.0, graphology-layout-forceatlas2 0.10.1 e graphology-communities-louvain 2.0.2. [Documentação de ForceAtlas2](https://graphology.github.io/standard-library/layout-forceatlas2.html), [documentação de Louvain](https://graphology.github.io/standard-library/communities-louvain.html), [licenças MIT incorporadas](LICENSES/Graphology.txt). Tudo está empacotado; não há download de bibliotecas durante o uso.

## 3. Gráficos secundários

- **Presença de variáveis × temas:** contagem por unidades de texto, autores ou menções. Inclui todas as variáveis reconhecidas antes dos filtros visuais. Zero significa ausência de menção, não ausência da variável no solo.
- **Similaridade entre temas:** Jaccard é a interseção dos conceitos dividida por sua união. Cosseno usa vetores de frequência por unidade com TF-IDF suavizado entre temas. Ambos variam de 0 a 1; temas sem conceitos aceitos ficam sem valor. São medidas de proximidade lexical, **não correlações entre variáveis experimentais**. A matriz usa todos os conceitos aceitos antes dos filtros visuais.
- **Conectividade e alcance:** os doze primeiros conceitos exibidos, ordenados por grau, autores ou menções. Este gráfico acompanha os filtros da rede.

As células permitem conferir termos compartilhados ou trechos correspondentes. SVG exporta a vista atual; JSON inclui configurações, posições, métodos e dados de origem; CSV exporta matrizes com a medida escolhida. Ajustes são locais e não alteram respostas. O cálculo acontece no navegador e não transmite os textos a serviços externos de inteligência artificial.


Tema da rede oferece sempre **Todos os temas** e **T1–T10** para qualquer participante autenticado, inclusive dentro das fichas. Todos os temas reúne os textos da turma ativa; escolher T1–T10 mostra aquele recorte, com os mesmos dados e algoritmos usados pelo administrador. Somente esta ficha (ou Minha ficha na página coletiva) restringe explicitamente a um autor. Os mapas de presença e similaridade continuam coletivos. Temas sem respostas ficam disponíveis e mostram rede vazia. A visualização não altera as permissões de edição: somente o titular e o administrador editam a ficha.

# A expedição do carbono

Plataforma UFAPE para ensino e revisão narrativa sobre matéria orgânica em solos do semiárido brasileiro.

[Abrir a aula](https://diogopaes1.github.io/aula-mos-ufape/) · [Dez fichas Word](MOS_10_fichas_alunos.zip)

Conteúdo público; cadastro com nome, e-mail e senha, sem confirmação por e-mail. Área de acesso com **Participante** (**Entrar** ou **Cadastrar**) e **Administrador**. Até vinte inscritos, dez titulares exclusivos e lista de espera. O professor sorteia e inicia; atribuições ficam bloqueadas. Sala aberta até o professor fechar, sem prazo fixo de doze horas. Apenas titular e administrador editam a ficha.

Dez temas, sessenta perguntas específicas, resposta livre até 3.000 caracteres com espaços. Enzimas no tema 7 e metagenômica no 8. Pesquisa inicial de duas horas; apresentação de até cinco minutos. As fichas revisadas apoiam a construção posterior do artigo.

GitHub Pages serve o conteúdo; Google Apps Script com planilha privada verifica permissões e guarda respostas. Não é necessário login Google. Não publicar credenciais ou dados privados neste repositório.

Administração em coluna única, cadastro em janela própria e atualização automática da lista. Antes do início, o professor pode atribuir/desatribuir missões e resetar o sorteio com confirmação. Depois do início, os titulares permanecem bloqueados e novos inscritos ocupam somente vagas livres. **Pausar atividades** suspende a escrita estudantil e mantém leitura, respostas e titulares; **Retomar atividades** libera novamente a escrita.

A sessão salva é recuperada após recarregar a página; falhas temporárias não apagam o acesso. A gravação na planilha atualiza apenas registros alterados, mantendo a trava e a proteção contra sobrescrita entre abas. Recusas temporárias da trava são repetidas com espera; conflitos de versões continuam exigindo comparação. A exportação administrativa não modifica as fichas. Aguarde a confirmação de gravação antes de atualizar uma aba com rascunhos.

Redes de coocorrência calculadas no navegador com vocabulário técnico, léxico derivado de [UD Portuguese Bosque r2.16](https://github.com/UniversalDependencies/UD_Portuguese-Bosque/tree/r2.16), licença [CC BY-SA 4.0](LICENSES/UD_Portuguese_Bosque.txt), e lista portuguesa [stopword](https://github.com/fergiemcdowall/stopword), licença [MIT](LICENSES/stopword.txt). O léxico foi convertido em formas/classes/lemmas, com regras locais de extração. Não é etiquetador contextual neural; termos podem ser omitidos. Comunidades lexicais não provam causalidade ou correção científica. Referência linguística: [Rademaker et al. 2017](https://aclanthology.org/W17-6523/).

Esferas maiores indicam mais termos distintos conectados entre as conexões exibidas. A área cresce com o grau, preservando um tamanho mínimo para seleção. Ocorrências e autores continuam disponíveis ao selecionar o termo. A mesma regra vale para redes individuais, coletivas e figuras exportadas.

O desafio da conta conectada recebe destaque discreto e atalho **Seu desafio** na página da turma. O cabeçalho identifica o e-mail. A troca de contas descarta respostas atrasadas da sessão anterior e reinicializa identidade e permissões.


A exploração da rede tem quatro seções numeradas: **rede dinâmica**, **presença das variáveis nos temas**, **similaridade lexical entre temas** e **conectividade/autores/menções**. Controles acima do gráfico: ForceAtlas2, LinLog, circular ou por comunidades; Louvain, modularidade gulosa ou componentes conectados; resolução, temas, tipos de termos, limite de conceitos e força mínima da aresta. Também há pausa, reorganização, arraste, deslocamento da vista, zoom e nomes dos nós.

Variáveis mencionadas são preservadas além do limite, incluindo urease, fosfatase, matéria orgânica do solo, carbono orgânico total (COT), carbono da biomassa microbiana (CBM) e respiração basal do solo (RBS). Substantivos genéricos isolados e palavras funcionais são filtrados; expressões específicas e siglas são normalizadas. O léxico foi corrigido para considerar todas as classes gramaticais. Candidatos adicionais exigem expressão composta recorrente.

Os mapas oferecem contagem por unidades, autores ou menções e similaridade Jaccard/cosseno TF-IDF. Essa similaridade descreve vocabulário compartilhado, não correlação entre resultados experimentais de artigos. As células mostram os conceitos ou trechos associados. SVG/JSON exportam a vista e os filtros atuais; CSV exporta as matrizes. Todo cálculo ocorre no navegador, com bibliotecas incorporadas. [Métodos e limites](METODOS_REDE.md) · [Licenças Graphology](LICENSES/Graphology.txt).


Tema da rede oferece sempre **Todos os temas** e **T1–T10** para qualquer participante autenticado, inclusive dentro das fichas. Todos os temas reúne os textos da turma ativa; escolher T1–T10 mostra aquele recorte, com os mesmos dados e algoritmos usados pelo administrador. Somente esta ficha (ou Minha ficha na página coletiva) restringe explicitamente a um autor. Os mapas de presença e similaridade continuam coletivos. Temas sem respostas ficam disponíveis e mostram rede vazia. A visualização não altera as permissões de edição: somente o titular e o administrador editam a ficha.

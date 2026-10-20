# A expedição do carbono

Plataforma UFAPE para ensino e revisão narrativa sobre matéria orgânica em solos do semiárido brasileiro.

[Abrir a aula](https://diogopaes1.github.io/aula-mos-ufape/) · [Dez fichas Word](MOS_10_fichas_alunos.zip)

Conteúdo público; cadastro com nome, e-mail e senha, sem confirmação por e-mail. Área de acesso com **Participante** (**Entrar** ou **Cadastrar**) e **Administrador**. Até vinte inscritos, dez titulares exclusivos e lista de espera. O professor sorteia e inicia; atribuições ficam bloqueadas. Sala aberta até o professor fechar, sem prazo fixo de doze horas. Apenas titular e administrador editam a ficha.

Dez temas, sessenta perguntas específicas, resposta livre até 15.000 caracteres com espaços. Enzimas no tema 7 e metagenômica no 8. Pesquisa inicial de duas horas; apresentação de até cinco minutos. As fichas revisadas apoiam a construção posterior do artigo.

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


No acesso à sala, o e-mail administrativo diogopaes.pnpd@ufape.edu.br deve usar Administrador. Se ele for informado em Participante, a janela orienta a troca de opção antes de enviar a senha. A conta de um participante não recebe poderes administrativos por usar a senha de outra conta.

Os campos de senha oferecem um olhinho interno para mostrar ou ocultar o texto digitado, inclusive no acesso, cadastro e troca de senha. A exibição começa oculta e não altera nem envia a senha.


Uma conta pode assumir vários temas. O professor usa **Adicionar tema** para ocupar uma missão livre, preservando as anteriores; cada tema mantém seis respostas, complementos, conclusão e versão próprios. Os temas existentes continuam bloqueados após iniciar e cada tema tem um único titular. Em Turma e sorteio, todos os temas próprios aparecem destacados; em Presença, a pessoa aparece uma vez com o progresso de suas perguntas e links para suas fichas. Nas redes, duas fichas da mesma conta contam como uma autoria.

As seis respostas e o campo de referências admitem até 15.000 caracteres cada, o esquema até 20.000 e a conexão até 10.000, incluindo espaços. Cada caixa mostra a contagem atual e o limite, atualizados ao digitar e associados ao campo para tecnologias assistivas. Os complementos têm área de escrita ampliada e ações de conclusão/gravação separadas por margem. As versões, a conclusão e as permissões de autoria continuam protegidas no servidor.

A rede agora distingue coocorrência textual e relações bibliográficas conferidas. São 72 relações tipificadas de 16 artigos, deduplicadas por DOI, com fonte, alcance e limite na inspeção e no CSV. A vista integrada preserva também resultados negativos, medidas conjuntas, fórmulas e hipóteses sem equipará-los a causalidade. Os filtros permitem recuperar apenas o texto original dos alunos ou examinar os complementos docentes identificados nas fichas. Nenhum texto anterior foi removido.

**Construir o artigo** apresenta a pergunta central sobre recuperação funcional dos solos da Caatinga, cinco seções complementares e tarefas por tema. Nomes e atribuições são consultados apenas na sessão autenticada; o HTML público não contém identidades dos estudantes; o DOCX nominal tem publicação autorizada pelo professor. Uma conta com dois temas aparece com as duas responsabilidades na mesma linha. O direcionamento pode ser baixado.

[Conferir métodos e limites da rede](METODOS_REDE.md). As relações de perda de solo se apoiam em estudo regional de Pesqueira, publicado em2023 com observações de2009–2010; não são tratadas como medidas de carbono ou microbiologia.


Materiais da reunião de21/10/2026: Construir o artigo oferece o direcionamento DOCX em Times New Roman, fontes pretas, recuo1,25cm e numeração1.; coleção completa em um ZIP com download conferido pelo navegador, com índiceR01–R17 e indicação de integral pendente. Arquivos em materiais/. Publicação desses materiais autorizada expressamente pelo professor.

## Exemplo que será editado após o levantamento de requisito.

Project Name> Equipe:Nome da Equipe
Projeto Integrador IV

























Documento de Requisitos do Sistema
<ProjectName>
Versão 1.0

Histórico de Alterações
Data	Versão	Descrição	Autor
17/01/2023	1.0	xxxxxxxxxxx	xxxxxx
			
			

Conteúdo
INTRODUÇÃO	4

1.1		VISÃO GERAL DO DOCUMENTO	4
1.2		CONVENÇÕES, TERMOS E ABREVIAÇÕES	4
	1.2.1	Identificação dos requisitos	4
	1.2.2	Prioridades dos requisitos	4

DESCRIÇÃO GERAL DO SISTEMA	5


1.	Introdução

Este documento especifica os requisitos do sistema Fast System Support, através de casos de uso, fornecendo aos desenvolvedores e cliente as informações necessárias para o projeto e implementação, assim como para a realização dos testes e homologação do sistema.

Visão geral do documento
Além desta seção introdutória, as seções seguintes estão organizadas como descrito abaixo.
Seção 2 – Descrição geral do sistema: apresenta uma visão geral do sistema, caracterizando qual é o seu escopo e descrevendo seus usuários.
Seção 3 – Requisitos funcionais (casos de uso): especifica todos os casos de uso do sistema, descrevendo os fluxos de eventos, prioridades, atores, entradas e saídas de cada caso de uso a ser implementado.
Seção 4 – Requisitos não-funcionais: especifica todos os requisitos não funcionais do sistema, divididos em requisitos de usabilidade, confiabilidade, desempenho, segurança, distribuição, adequação a padrões e requisitos de hardware e software.

Convenções, termos e abreviações
A correta interpretação deste documento exige o conhecimento de algumas convenções e termos específicos, que são descritos a seguir.

FSS - Fast System Support
Frame – É um elemento que permite exibir o conteúdo extra dentro de uma página.

Identificação dos requisitos
Por convenção, a referência a requisitos é feita através do nome da subseção onde eles estão descritos, seguidos do identificador do requisito, de acordo com a especificação a seguir:
[nome da subseção. identificador do requisito]
Por exemplo, o requisito funcional [Recuperação de dados.RF016] deve estar descrito em uma subseção chamada “Recuperação de dados”, em um bloco identificado pelo número [RF016]. Já o requisito não-funcional [Confiabilidade.NF008] deve estar descrito na seção de requisitos não-funcionais de Confiabilidade, em um bloco identificado por [NF008].
Os requisitos devem ser identificados com um identificador único. A numeração inicia com o identificador [RF001] ou [NF001] e prossegue sendo incrementada à medida que forem surgindo novos requisitos.

Prioridades dos requisitos
Para estabelecer a prioridade dos requisitos, na seção 4, foram adotadas as denominações “essencial”, “importante” e “desejável”.
Essencial é o requisito sem o qual o sistema não entra em funcionamento. Requisitos essenciais são requisitos imprescindíveis, que têm que ser implementados impreterivelmente.

Importante é o requisito sem o qual o sistema entra em funcionamento, mas de forma não satisfatória. Requisitos importantes devem ser implementados, mas, se não forem, o sistema poderá ser implantado e usado mesmo assim.
Desejável é o requisito que não compromete as funcionalidades básicas do sistema, isto é, o sistema pode funcionar de forma satisfatória sem ele. Requisitos desejáveis podem ser deixados para versões posteriores do sistema, caso não haja tempo hábil para implementá- los na versão que está sendo especificada.
2.	Descrição geral do sistema


2.1	Abrangência e sistemas relacionados
A competitividade e a velocidade da evolução do mercado cada vez mais demandam novas estratégias de negocio que visam aproximar cliente e empresa. A velocidade de reposta é uma técnica fundamental para satisfação do cliente e de forma geral um fator de competitividade que pode ser alcançado com a informatização do atendimento ao cliente.

O FSS é uma ferramenta que intermédia a relação cliente/empresa com o intuito não somente de solucionar problemas, mas como solucioná-los de forma rápida garantindo a satisfação do cliente.

Com uma intuitiva, eficiente e de fácil acesso interface WEB, o usuário pode sanar suas dúvidas, resolver problemas e levantar críticas ou sugestões.

A ferramenta também disponibiliza a funcionalidade de consulta de histórico de atendimento, permitindo ao usuário o cumprimento da obrigação levantada pelo atendente.

3. Requisitos funcionais (casos de uso)



Cadastro

<INSERIR AQUI DIAGRAMAS DE CASO DE USO DE CADASTRO>

[RF001] Selecionar Perfil

Descrição do caso de uso: Este caso de uso permite ao sistema disponibilizar atendentes aos futuros usuários do sistema.

Ator: Atendente

Prioridade:	■ Essencial	Importante	Desejável
Entradas e pré-condições: Atendente estar cadastrado no sistema.

Saídas e pós-condição: Está disponível para atendimento aos usuários.


[RF002] Preencher Nome e E-mail

Descrição do caso de uso: Este caso de uso permite aos usuários informar os dados solicitados pelo sistema para realizar o atendimento.
Ator: Cliente

Prioridade:	■ Essencial	Importante	Desejável

Entradas e pré-condições: Usuário acessar o sistema.

Saídas e pós-condição: O usuário é direcionado para a tela de seleção de atendentes disponíveis.
[RF003] Escolher Atendente Disponível

Descrição do caso de uso: Este caso de uso permite que o usuário escolha um atendente disponível para realizar o atedimento.

Ator: Cliente

Prioridade:	■ Essencial	Importante	Desejável

Entradas e pré-condições: RF[002]

Saídas e pós-condição: Tela de espera.

[RF004] Aceitar ou Recusar Atendimento

escrição do caso de uso: Este caso de uso permite que o atendente aceite ou recuse a solicitação de atendimento do usuário.

Ator: Atendente

Prioridade:	■ Essencial	Importante	Desejável

Entradas e pré-condições: RF[003]

Saídas e pós-condição: Caso aceite será direcionado para uma tela de atendimento ao cliente, caso contrario o atendente permanece na tela atual.

[RF005] Realizar Atendimento

Descrição do caso de uso: Este caso de uso permite a interação entre atendente e usuário.

Ator: Atendente

Prioridade:	■ Essencial	Importante	Desejável

Entradas e pré-condições: RF[004*]

Saídas e pós-condição: Realizar o atendimento.






[RF006] Consultar Histórico de Atendimento

Descrição do caso de uso: Este caso de uso permite a consulta do atendimento realizado ao cliente mediante a apresentação da chave correspondente ao mesmo.

Ator: Cliente

Prioridade:	Essencial	■ Importante	Desejável

Entradas e pré-condições: Chave única do atendimento.

Saídas e pós-condição: A tela com o histórico de atendimento.


[RF007] Histórico Resumido de Atendimentos

Descrição do caso de uso: Este caso de uso permite que seja exibido na tela inicial do atendente o histórico resumido dos atendimentos realizados.

Ator: Atendente

Prioridade:	Essencial	■ Importante	Desejável

Entradas e pré-condições: O atendente deve estar conectado no seu perfil.

Saídas e pós-condição: Resumo com o nome e-mail e data do atendimento.



[RF008] Detalhes de Atendimento

Descrição do caso de uso: Este caso de uso permite que seja visualizado os detalhes como nome, e-mail, data/hora do inicio e termino do atendimento e dialogo entre atendente e cliente.

Ator: Atendente

Prioridade:	Essencial	■ Importante	Desejável

Entradas e pré-condições: Selecionar o atendimento que deseja visualizar.

Saídas e pós-condição: Tela com os detalhes de atendimento.

Interface

<INSERIR AQUI DIAGRAMAS DE CASO DE USO DE INTERFACE>
[RF001] Visualizar Componente

Descrição do caso de uso: Este caso de uso permite que o usuário visualize os dados de um determinado componente (todos os seus atributos, exceto aqueles que são considerados suas propriedades).

Prioridade:	Essencial	■ Importante	Desejável
Entradas e pré-condições: deve receber como entrada o componente que se
deseja visualizar.

Saídas e pós-condição: o usuário visualiza o componente desejado
[RF002] Copiar componente

Descrição do caso de uso: Este caso de uso permite que o usuário copie um componente do cadastro de componentes do sistema. Ou seja, copia o componente de onde ele estava e manda a cópia para a área de transferência.

Prioridade:	■ Essencial	Importante	Desejável
Entradas e pré-condições: recebe como entrada o componente que se deseja
copiar.

Saídas e pós-condição: o usuário consegue copiar o componente que deseja
[RF003] Colar componentes

Descrição do caso de uso: Este caso de uso permite que o usuário cole o componente armazenado na área de transferência do sistema no local indicado. O conteúdo da área de transferência continua inalterado. Aqui, local refere-se a uma pasta que contém componentes.

Prioridade:        ■ Essencial	Importante	Desejável

Entradas e pré-condições: recebe como entrada o componente que se deseja colar e tem como pré-condição a necessidade de existência de alguma informação na área de transferência do sistema.

Saídas e pós-condição: o usuário consegue colar o componente no local desejado.

Compilação

<INSERIR AQUI DIAGRAMAS DE CASO DE USO>

[RF001] Compilar componente

Descrição do caso de uso: Este caso de uso permite que o usuário compile metodologias. Essa compilação permite que as metodologias sejam analisadas e comparadas entre si.

Prioridade:	Essencial	■ Importante	Desejável

Entradas e pré-condições: deve receber como entrada as metodologias a serem compiladas.

Saídas e pós-condição: os componentes das metodlogias são compilados no sistema.

Importação/Exportação

[RF001] Anexar documentos

Descrição do caso de uso: Este caso de uso permite que anexar documentos gerais a componentes. Por exemplo, anexar o template do Documento de Requisitos ao fluxo de requisitos.

Prioridade:	Essencial	■ Importante	Desejável

Entradas e pré-condições: deve receber como entrada o caminho absoluto para um arquivo no sistema de arquivos.

Saídas e pós-condição: O documento é anexado ao componente.
[RF002] Exportar metodologia

Descrição do caso de uso: Este caso de uso permite ao usuário a possibilidade de exportar uma metodologia num determinado formato, como XML, por exemplo. O usuário também tem a opção de escolher se o componente deve ou não ser exportado juntamente com seus anexos.

Prioridade:        ■ Essencial	Importante	Desejável

Entradas e pré-condições: A entrada é uma metodologia a ser exportado e seus sub-componentes, ou seja, todos os componentes que um determinada metodologia.

Saídas e pós-condição: Os componentes são exportados para um arquivo em um determinado formato (como XML).
[RF003] Importar metodologia

Descrição do caso de uso: Este caso de uso permite que componentes de uma metodologia exportada sejam importados do sistema de arquivos e apresentados no Methodology Explorer. Os componentes, para serem importados precisam estar no mesmo formato utilizado no caso de uso [Importação/Exportação.RF002]. Importar um componente apenas permite manipular o componente dentro do Methodology Explorer. Para inseri-lo de fato, é preciso realizar o caso de uso [Importação/Exportação.RF004]

Prioridade:        ■ Essencial	Importante	Desejável

Entradas e pré-condições: A entrada é o caminho absoluto para um arquivo no sistema de arquivos.

Saídas e pós-condição: O componente importado será inserido na(s) árvore(s) de componentes adequada.
[RF004] Salvar metodologia

Descrição do caso de uso: Este caso de uso permite salvar as alterações realizadas nos componentes de uma metodologia.

Prioridade:	Essencial	■ Importante	Desejável

Entradas e pré-condições: A entrada é uma metodologia.

Saídas e pós-condição: um componente é persistido no Methodology Explorer.
[RF005] Gerar site de metodologia

Descrição do caso de uso: Este caso de uso permite que um site seja gerado para uma metodologia já compilada. O site deve conter também os possíveis artefatos que foram anexados.

Prioridade:	Essencial	■ Importante	Desejável

Entradas e pré-condições: Um componente metodologia é a entrada para o caso de uso que tem, como pré-condição, que a toda a metodologia já esteja salva.

Saídas e pós-condição: um site completo é gerado no sistema de arquivos contendo os arquivos HTML e os artefatos anexados à metodologia.

4.	Requisitos não-funcionais

Usabilidade Portabilidade Desempenho
Não Roda no Internet Explorer
[NF001] Usabilidade

A interface com o usuário é de vital importância para o sucesso do sistema. Principalmente por ser um sistema que não será utilizado diariamente, o usuário não possui tempo disponível para aprender como utilizar o sistema.
O sistema terá uma interface amigável ao usuário primário sem se tornar cansativa aos usuários mais experientes. Em especial, o módulo de publicação HTML possuirá um wizard para ajudar o usuário.


Prioridade:        ■ Essencial	Importante	Desejável

[NF002] Desempenho

Embora não seja um requisito essencial ao sistema, deve ser considerada por corresponder a um fator de qualidade de software.

Prioridade:	Essencial	■ Importante	Desejável

[NF003] Hardware e Software

Visando criar um produto com maior extensibilidade, reusabilidade e flexibilidade, deve ser adotar como linguagem principal de desenvolvimento Java seguindo cuidadosamente as técnicas de orientação a objetos. Entretanto, outras linguagens também poderão ser usadas quando indicações técnicas recomendem.
O uso da linguagem Java permite não especificar qual será o sistema operacional e a máquina em que o programa irá executar. No entanto, essa máquina deverá se comunicar com um sistema de banco de dados.

Prioridade:	Essencial	■ Importante	Desejável

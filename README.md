O Observer é um padrão de projeto de software que define uma dependência um-para-muitos entre objetos de modo que quando um objeto muda o estado, todos seus dependentes são notificados e atualizados automaticamente. Permite que objetos interessados sejam avisados da mudança de estado ou outros eventos ocorrendo num outro objeto.

O padrão Observer é também chamado de Publisher-Subscriber, Event Generator e Dependents.

Motivação

Um objeto que possua agregações deve permitir que seus elementos sejam acessados sem que a sua estrutura interna seja exposta.

Descrição de um problema

Para esse problema, uma solução poderia ser manter uma lista com as possíveis representações e ficar verificando por mudanças nos conjuntos de dados, assim que fosse feita mudança, as representações que está na lista seriam avisadas. Portanto, o padrão Observer resolve esse problema.

Como garantir que objetos que dependem de outro objeto percebam as mudanças naquele objeto?

Os observadores devem conhecer o objeto de interesse. O objeto de interesse deve notificar os observadores quando for atualizado.

Aplicabilidade

Quando uma mudança a um objeto requer mudanças a outros e você não sabe quantos outros objetos devem mudar ou quando um objeto deve ser capaz de avisar outros sem fazer suposições sobre quem são os objetos.

Consequências

Possibilita baixo acoplamento entre os objetos dependentes e o assunto.

Conclusão


O padrão Observer é uma excelente opção para códigos como o do exemplo apresentado ou códigos com listeners de eventos em geral.

Um objeto tendo de notificar mais do que um outro objeto, nesse caso o Observer é o código a ser implementado. Além do mais, é um padrão simples de entender e utilizar.

Quando implementando o padrão, busque a maneira mais otimizada, ou seja, como apresentado no artigo, a versão "puxar" tende a ser mais eficiente.

O que é Artecoin?
Artecoin é uma moeda digital experimental que permite pagamentos instantâneos para qualquer pessoa, em qualquer lugar do mundo. Artecoin utiliza tecnologia peer-to-peer para operar sem uma autoridade central: o gerenciamento de transações e a emissão de dinheiro são realizados coletivamente pela rede. Artecoin Core é o nome do software de código aberto que permite o uso dessa moeda.

Para mais informações, assim como uma versão binária imediatamente utilizável do software Artecoin Core, veja https://artecoin.org.

Licença
Artecoin Core é lançado sob os termos da licença MIT. Veja COPYING para mais informações ou acesse https://opensource.org/licenses/MIT.

Processo de Desenvolvimento
A branch master é regularmente construída (veja doc/build-*.md para instruções) e testada, mas não é garantido que seja completamente estável. Tags são criadas regularmente a partir de branches de lançamento para indicar novas versões oficiais e estáveis do Artecoin Core.

O repositório https://github.com/seu-usuario/gui é usado exclusivamente para o desenvolvimento da GUI. Sua branch master é idêntica em todos os repositórios monotree. Branches de lançamento e tags não existem, então, por favor, não faça fork desse repositório, a menos que seja por razões de desenvolvimento.

O fluxo de trabalho de contribuição é descrito em CONTRIBUTING.md e dicas úteis para desenvolvedores podem ser encontradas em doc/developer-notes.md.

A lista de discussão para desenvolvedores deve ser usada para discutir mudanças complicadas ou controversas antes de trabalhar em um conjunto de patches.

O IRC para desenvolvedores pode ser encontrado no Freenode em #artecoin-dev.

Testes
Testes e revisão de código são o gargalo para o desenvolvimento; recebemos mais pull requests do que podemos revisar e testar em curto prazo. Por favor, seja paciente e ajude testando pull requests de outras pessoas, e lembre-se de que este é um projeto crítico para a segurança onde qualquer erro pode custar muito dinheiro para as pessoas.

Testes Automatizados
Os desenvolvedores são fortemente encorajados a escrever testes unitários para o novo código e a submeter novos testes unitários para o código antigo. Testes unitários podem ser compilados e executados (assumindo que não foram desativados na configuração) com: make check. Mais detalhes sobre como executar e estender testes unitários podem ser encontrados em /src/test/README.md.

Existem também testes de regressão e integração, escritos em Python, que são executados automaticamente no servidor de build. Esses testes podem ser executados (se as dependências de teste estiverem instaladas) com: test/functional/test_runner.py

O sistema Travis CI garante que cada pull request seja construído para Windows, Linux e macOS, e que testes unitários/sanitários sejam executados automaticamente.

Testes de Garantia de Qualidade (QA) Manuais
As mudanças devem ser testadas por alguém que não seja o desenvolvedor que escreveu o código. Isso é especialmente importante para mudanças grandes ou de alto risco. É útil adicionar um plano de teste à descrição do pull request se testar as mudanças não for algo direto.

Traduções
Nós aceitamos apenas correções de tradução que sejam submetidas através da página do Transifex do Bitcoin Core. As traduções são convertidas periodicamente para o Artecoin.

As traduções são periodicamente puxadas do Transifex e mescladas no repositório git. Veja o processo de tradução para detalhes sobre como isso funciona.

Importante: Não aceitamos mudanças de tradução como pull requests no GitHub porque a próxima extração do Transifex as sobrescreveria automaticamente.


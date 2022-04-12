- O Git considera cada `commit`ponto de alteração do seu projeto, fazendo assim um histórico do seu trabalho ao longo do desenvolvimento.

- Uma boa mensagem de commit deve conter a descrição do que foi feito e para nos ajudar, podemos utilizar este **padrão de escrita das mensagens.**

- Cada mensagem de confirmação consiste em um **cabeçalho que é obrigatório**, um **corpo** e um **rodapé (estes são opcionais)** . O cabeçalho tem um formato especial que inclui um **tipo**, um **escopo** e uma descrição:

  ```
  <tipo>[escopo opcional]: <descrição> 
  [corpo opcional] 
  [rodapé(s) opcional(is)]
  ```

  > Tipos:
  >
  > - **fix** — Commits do tipo `fix` indicam que seu trecho de código commitado está solucionando um problema (bug fix).
  > - **feat** — Commits do tipo `feat` indicam que seu trecho de código está incuindo um novo recurso.
  > - **test** — Commits do tipo `test` são utilizados quando são realizadas alterações em testes, seja criando, alterando ou excluindo testes unitários. *(Não inclui alterações em código)*
  > - **docs** — Commits do tipo `docs` indicam que houveram mudanças na documentação, como por exemplo no Readme do seu repositório. *(Não inclui alterações em código).*

**Commit semântico com tipo e descrição**

```
docs: ortografia correta de CHANGELOG
```

```
fix: solução do bug no footer
```

```
feat: inserção do formulário, com as respectivas regras
```



**Corpo do commit**

O **corpo**, como mencionado no “esqueleto do commit semântico” é opcional. É indicado utilizá-lo quando o detalhamento do seu commit irá ser maior que 7 palavras.

**Commit semântico com corpo**

```
feat: adicionado a nova estrutura de pastas do frontend
- Foi realizada uma mudança em toda a estruturação de páginas do projeto frontend,
pois agora iremos utilizar o modelo de Design Atômico.
```



**Escopo do cabeçalho (opcional)**

O escopo do commit, é opcional, e é com ele que iremos informar qual parte do código foi modificado.

**Commit Semântico com escopo e corpo**

```
fix(ProdutoApi): retirando variável do path da API e ajustando loggers
- O path anterior tinha variáveis desnecessárias e não utilizadas por nenhum
consumidor
```



**Rodapé (opcional)**

O **rodapé,** assim como o **escopo e descrição**, são opcionais de serem informados. Nele geralmente são informados uma issue, id ou tasks de atividades, que foram utilizadas para realizar a alteração desse trecho de código commitado.

```
fix: corrige pequenos erros de digitação no código
- veja o ticket para detalhes sobre os erros de digitação corrigidos.originado da issue JD#12.
```
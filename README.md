# 🌻 **Siga o FLOW para trabalhar no projeto**


## **🔀 Para começar**
Crie um  `clone` do repositório no seu ambiente de desenvolvimento, você pode usar seu terminal de preferência (GitBash, cmd):

Clonando repositório

```Bash
# git clone [url-do-dorepositório]
$ git clone https://MoroniPereira@bitbucket.org/santriweb/ecommerce.git
```

Para demais configurações como arquivo env, banco de dados e docker, consulte um administrador do projeto.


## **✏️ Realizando as modificações**
A primeira coisa a se fazer é criar uma branch com o código do seu card. O nome da branch deve ser `exatamente` igual ao código do card. 

Brancho a branch:
```Bash
# git checkout -b [codigo-do-card]
$ git checkout -b ESW-1195
```

Tipo de alteração:
- feature: adiciona nova funcionalidade
- chore: altera uma funcinoalidade existente
- fix: resolve um problema

## **💾 Staged -> Commit**
A cada etapa concluída da sua alteração é aconselhado realizar um "commit". Isso serve para que você possa apagar o que está fazendo e ainda manter as alterações anteriores.

Siga essa etapas:

Veja uma lista dos arquivos modificados
```Bash
$ git status
```

Envie os arquivos que você queira realizar o commit
- Não é aconselhado usar o `git add .(all)`
```Bash
$ git add src/styles/
```

Realize o commit das mudanças. Nós também temos um padrão de commit.

```Bash
$ git commit -m "[codigo-do-card] - [tipo-de-mudança]: [descrição]"
$ git commit -m "ESW-1165 - FEATURE: Criando um novo id no css dedicado ao componente criado"  
```
[Leia mais sobre o padrão de commit](https://dev.to/renatoadorno/padroes-de-commits-commit-patterns-41co)

Tipo de mudança (principais):
  - chore - mudanças em arquivos que já são controlados pelo git.
  - feat - adicionando uma nova funcionalidade, módulo, etc.
  - fix - realiza alguma correção no código.
  - refactor - realiza modificações no código sem adicionar ou alterar o comportamento do código.

A descrição do commit devem deixar explícito a principal alteração no código:

- ❌ Exemplo errado:
  - "chore: alteraçãos no arquivo .gitignore"
- ✅ Exemplo correto:
  - "chore: inclui o arquivo .env no .gitignore"

## **🔄 Sincronizando as branchs**
Após realizar todas as suas alterações e commitar, chegou a hora de dar pull na branch remota.
Dentro da branch local criada para sua demanda, rode o comando:

```Bash
$ git pull origin [codigo-do-card]
$ git pull origin ESW-1165
```

## **🔃 Pull-request**
Acesse seu repositório no GitHub, acesse a branch que acabou de enviar e crie um pull-request
<img width="75%" src="https://user-images.githubusercontent.com/48590313/241337789-2d2f5013-affa-4769-ac45-8c4e86abdba3.png" />
<img width="75%" src="https://user-images.githubusercontent.com/48590313/241337798-bb5b0fac-d732-4415-9dcd-1a27b8f23b5e.png" />

## **🎊 Congratulations!**
Adicione a descrição da pull-request detalhando todas as alterações que ela faz e envie a requisição.
> 🆙 Nessa etapa, a descrição pode ser no seu idioma de domínio para que a escrita fique melhor, o meu é português brasileiro.

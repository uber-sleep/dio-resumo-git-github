
# Comandos Git e Github

Principais comandos Git e Github.


## Documentação

- [Documentação Git](https://git-scm.com/docs/git/pt_BR)
- [Documentação Github](https://docs.github.com/pt)



## Resumo 
### Configurações Iniciais

| Comandos  | Explicação |
| ------------- | ------------- |
| git config --global user.name "[firstname lastname]"| indica o nome de usuario para o Git e para futuras revisoes. |
| git config --global user.email “[valid-email]”  | indica o email do usuario para o Git e para futuras revisoes.  |
|git config --global color.ui | seleciona a cor para facilitar a revisão.

### Configurações e Inicialização
|Comandos | Explicação |
|-------------|-------------|
|git init | inicializa um repositorio ja existente no git |
|git clone [url] | busca e clona um repositorio do github |

### Slavando Alterações
|Comandos | Explicação |
|-------------|-------------|
| git status | mostra o status dos arquivos no diretório atual |
| git add [file] | adiciona o arquivo ao stage, prepara para o commit |
| git add . | adiciona todos os arquivos nao modificados para a area de stage |
| git commit -m "[descrição]" | faz o commit dos arquivos em stage |
| git log | mostra todos os commits da branch atual |

### Desfazendo Alterações
|Comandos | Explicação |
|-------------|-------------|
| rm -rf .git | remove o diretorio .git do seu conteúdo a força |
| git restore [file] | descarta todas as alterações feitas localmente |
| git --amend -m "[mensagem corrigida]" | corrige a mensagem do último commit |
| git commit --amend (:wq pra sair) | abre o editor de commit |
| git reset --soft [commit]	| Desfaz o commit mantendo as alterações no stage |
| git reset --mixed [commit] | Desfaz o commit e remove as alterações do stage, mantendo as alterações nos arquivos locais |
| git reset --hard [commit]	| Desfaz o commit e descarta todas as alterações, revertendo para o estado do commit especificado |
| git reset [file] | Remove o arquivo do stage, desfazendo as alterações no arquivo, mas mantendo as alterações nos arquivos locais |
| git restore --staged [file] | Desfaz a adição do arquivo ao stage, revertendo para o estado anterior à adição |
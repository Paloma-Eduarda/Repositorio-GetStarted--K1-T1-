##Comandos Git
---

###Comandos básicos

Alterar a Branch

    git config --global init.defaultBranch master

Criar repositório git
    
    git init

status do repositório
    
    git status
    
Para adicionar todos os arquivos
   
    git add --all
    git add .
    git add -A
   
Para adicionar um arquivo específico

    git add "nome do arquivo"
   
Para fazer com que um arquivo não seja mais rastreado pelo git (senhas)
   
    git rm -- cached nome_arquivo
Para remover todos os arquivos
    
    git rm --cached -r .

Dando commit
  
    git commit -m 'mensagem_para_gravar'

**Visualizar Alterações**

Verificar as alterações que foram feitas nos arquivos antes de adicionar novamente Unmodified - modified

    git diff"
    
Quando os 2 arquivos estão alterados, estado = modified
    
    git diff --cached" ou "git diff --staged

**Histórico de Commit**

Para ver o histórico do git
    
    git log
Para ver apenas algumas informações como, mensagem gravada e código commit
    
    git log --oneline
Você também pode escolher quantos commit ver
    
    git log -numero_de_commits
    
Da para juntar mais de um comando
    
    git log --oneline -numero_de_commits
    
Para ver o historico em uma branch específica
    
    git log nome_da_branch --oneline

Para ver o histórico + atualizações
    
    git log -p
Ver modificações e quem as fez
    
    git log --stat

**Alteração de commit**

Alterar mensagem salva
    
    git commit --amend -m "nova_mensagem

Usando commits anteriores
    
    git checkout codigo_comite

Desfazer alterações

*reverter arquivos para ultima versão para última conhecida do commit*
*Arquivo Tracked/modified*

    git checkout nome_arquivo.txt
    git checkout .


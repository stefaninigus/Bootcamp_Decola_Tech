# Anotações sobre uso de terminal, Git e GitHub em dispositivos android
 - ## Terminal
####  -para utilizar o terminal em dispositivos androids é necessário a emular um ambiente linux, podendo ser feito via aplicativo Termux
####  -após baixar e instalar o Termux pela PlayStore basta iniciar o programa e, por rotina de checagem, atualizá-lo por completo com *apt update && apt upgrade*
####  -o Termux terá um diretório próprio, porém para q ele tenha acesso a arquivos externos (internal Storage do dispositvo ou cartão SD e similares) é necessário rodar o comando *termux-setup-storage* e ativar as permissões do sistema de acesso ao armazenamento
 - ## Git
####  -para instalação do Git via Termux basta rodar o comando *pkg install git* e este será instalado conforme versão disponibilizada no repositório padrão do Termux
####  -é recomendado também instalar o SSH (*pkg install openssh*) para conexão com GitHub futuramente
 - ## GitHub
####  -para logar no GitHub é necessário estar setada uma chave ssh
####  -tendo instalado o openssh isso pode ser feito usando o comando *ssh-keygen -t rsa -C EMAIL*
####  -uma vez gerada a chave basta cadastrar a versão pública na sua conta no GitHub e, após, autenticar com o comando *ssh -T git@github.com*
 - ## Conclusão
####  -todos os comandos Git e comandos de terminal linux funcionarão normalmente, e o fluxo se manterá relativamente igual a utilização em computadores
####  -irei relatar alguns comandos a serem mais usados para facilitar o processo ao longo do Desafio 1 do Bootcamp
 - ##### *clear*                     /limpa a tela do termux
 - ##### *cd <>*                     /muda para diretório especificado
 - ##### *mkdir <>*                  /cria novo diretório
 - ##### *rm -rf <>*                 /deleta diretório especificado
 - ##### *ls*                        /lista arquivos e diretórios
 - ##### *git config -l*             /lista configurações setadas no git
 - ##### *git --global <>*           /seta configuração especificada
 - ##### *git init*                  /inicializa git no diretório
 - ##### *git status*                /relata a situação do diretório e stage em relação ao commit mais recente e dá dicas do que fazer a seguir
 - ##### *git remote origin "URL"*   /conecta repositório local ao repositório no github
 - ##### *git push origin master*    /empurra o repositório ao github
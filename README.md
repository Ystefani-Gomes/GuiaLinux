# GuiaLinux
# Guia de Comandos para Administração de Servidores Linux

Este repositório contém um guia prático e conciso com comandos essenciais de Linux para a administração de servidores.

---

## Sumário (TOC)

---

## 1. Comandos de Navegação e Diretórios

Comandos usados para se mover e gerenciar a estrutura de pastas e arquivos.

| Comando | Descrição | Exemplo de Uso |
| :--- | :--- | :--- |
| **pwd** | Imprime o nome do diretório de trabalho atual. | pwd |
| **ls** | Lista o conteúdo de um diretório. | ls -lha |
| **cd** | Muda o diretório de trabalho. | cd /var/log |
| **mkdir** | Cria novos diretórios (pastas). | mkdir novos_dados |
| **rmdir** | Remove diretórios vazios. | rmdir lixo |
| ... | (Adicione mais comandos de navegação aqui) | ... |

---

## 2. Comandos de Manipulação de Arquivos

Comandos essenciais para criar, copiar, mover e deletar arquivos.

| Comando | Descrição | Exemplo de Uso |
| :--- | :--- | :--- |
| **touch** | Cria um novo arquivo vazio. | touch meu_arquivo.txt |
| **cp** | Copia arquivos e diretórios. | cp arq1.conf /etc/ |
| **mv** | Move ou renomeia arquivos e diretórios. | mv arq1.txt arq_final.txt |
| **rm** | Remove (deleta) arquivos e diretórios. | rm -rf pasta_antiga |
| **cat** | Exibe o conteúdo de um arquivo. | cat /etc/passwd |
| **less** | Exibe o conteúdo de um arquivo em tela por tela. | less grande_log.txt |
| ... | (Adicione mais comandos de manipulação aqui) | ... |

---

## 3. Comandos de Gerenciamento de Sistema e Processos

Comandos para monitorar o sistema, memória e processos ativos.

| Comando | Descrição | Exemplo de Uso |
| :--- | :--- | :--- |
| **top** | Exibe processos e uso de recursos em tempo real. | top |
| **ps** | Lista os processos ativos. | ps aux |
| **kill** | Envia um sinal para terminar um processo. | kill -9 1234 |
| **df** | Exibe o uso de espaço em disco. | df -h |
| **du** | Estima o uso de espaço em disco de um arquivo/diretório. | du -sh /home/user |
| ... | (Adicione mais comandos de sistema aqui) | ... |

---
---

## 4. Comandos de Rede

Comandos para configurar, verificar e diagnosticar problemas de rede.

| Comando | Descrição | Exemplo de Uso |
| :--- | :--- | :--- |
| **ip addr** | Exibe endereços IP e informações da interface de rede. | ip addr show eth0 |
| **ping** | Testa a conectividade entre dois hosts. | ping google.com |
| **ss** | (Socket Statistics) Exibe informações de sockets (substituto do netstat). | ss -tuln |
| **ssh** | Cliente para conexão remota segura. | ssh user@192.168.1.10 |
| **wget** | Baixa arquivos de um servidor web ou FTP. | wget http://site.com/file.zip |
| **curl** | Ferramenta para transferir dados com sintaxe de URL. | curl -I https://google.com |
| **hostname** | Exibe ou define o nome do host do sistema. | hostname |
| **traceroute** | Rastreia a rota dos pacotes de rede até um destino. | traceroute google.com |

---

## 5. Comandos de Usuários e Permissões

Comandos para gerenciar contas de usuário e controlar o acesso a arquivos.

| Comando | Descrição | Exemplo de Uso |
| :--- | :--- | :--- |
| **useradd** | Cria uma nova conta de usuário. | useradd -m novo_usuario |
| **passwd** | Altera a senha de um usuário. | passwd novo_usuario |
| **usermod** | Modifica as propriedades de uma conta de usuário. | usermod -aG sudo novo_usuario |
| **userdel** | Remove uma conta de usuário e seus arquivos. | userdel -r usuario_antigo |
| **chown** | Altera o proprietário (usuário e grupo) de um arquivo/diretório. | chown -R www-data:www-data /var/www/html |
| **chmod** | Altera as permissões de acesso de um arquivo/diretório. | chmod 755 script.sh |
| **groups** | Exibe os grupos aos quais um usuário pertence. | groups meu_usuario |
| **su** | Troca o usuário atual. | su - outro_user |
| **sudo** | Executa um comando como superusuário. | sudo apt update |

---

## 6. Comandos de Busca e Filtragem

Comandos usados para encontrar arquivos ou filtrar conteúdo dentro de arquivos.

| Comando | Descrição | Exemplo de Uso |
| :--- | :--- | :--- |
| **grep** | Procura por padrões dentro de arquivos. | grep "erro" /var/log/syslog |
| **find** | Procura por arquivos em um diretório. | find /home -name "*.log" |
| **locate** | Localiza arquivos usando um banco de dados pré-indexado (mais rápido). | locate config.conf |
| **which** | Mostra o caminho completo de um comando. | which bash |
| **head** | Exibe as primeiras linhas de um arquivo. | head -n 10 meu_log.txt |
| **tail** | Exibe as últimas linhas de um arquivo (ótimo para logs em tempo real). | tail -f /var/log/apache2/error.log |
| **sort** | Ordena linhas de arquivos de texto. | cat lista.txt | sort |
| **wc** | Conta linhas, palavras e caracteres de um arquivo. | wc -l lista.txt |
| **sed** | Editor de fluxo para filtrar e transformar texto. | sed 's/antigo/novo/g' arquivo.txt |

---

## 7. Comandos de Gerenciamento de Software e Sistema

Comandos para instalar, atualizar, desligar e reiniciar o sistema.

| Comando | Descrição | Exemplo de Uso |
| :--- | :--- | :--- |
| **apt update** | Atualiza a lista de pacotes disponíveis. | sudo apt update |
| **apt install** | Instala novos pacotes de software. | sudo apt install nginx |
| **systemctl** | Gerencia e interage com serviços do sistema (systemd). | sudo systemctl status apache2 |
| **shutdown** | Desliga o sistema. | sudo shutdown now |
| **reboot** | Reinicia o sistema. | sudo reboot |
| **history** | Exibe o histórico de comandos digitados. | history |
| **alias** | Cria atalhos para comandos longos. | alias l='ls -lha' |

---

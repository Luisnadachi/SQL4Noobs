# **Instalando SQL (MySQL)**

## **Observações**
Nesse repositório para explicar sobre SQL vamos está instalando o MySQL com o intuito de com ele mostrar o SQL, caso você queira se aprofundar mais em MySQL temos no 4noobs um [repositório](https://github.com/paulorievrs/mysql4noobs) feito pelo [Paulo Rivers](https://github.com/paulorievrs) falando sobre. Com a permissão dele algumas partes aqui da instalação eu tirei do repositório dele por conta de eu já ter instalado em meu windows o MySQL.  

## **Windows**

Caso você esteja utilizando o windows, só seguir os seguintes passos:

1. Acesse o site oficial do [MySQL](https://www.mysql.com)
2. Vá em Downloads
3. Procure o link para baixar MySQL Community
4. Clique em "MySQL Installer for Windows"
5. Escolha a opção "Windows (x86, 32-bit), MSI Installer"
6. Continue o Download sem criar conta
7. Execute o instalador, aceite os termos e avançe
8. Escolha o padrão desenvolvedor
9. Vai ocorrer uma verificação para baixar as dependências, clique em executar para instalar os pacotes necessários
10. Em seguida execute a instalação dos pacotes
11. Na próxima tela deixe em "Standalone MySQL Server / Classic MySQL Replication" 
12. Próxima tela vai ser as configurações padrões, pode avançar
13. Tela seguinte vai ser de autenticação, só seguir
14. Nessa tela, escolhe uma senha para o seu MySQL e guarde ela, avançe
15. Nessa tela mostra como ira ocorrer o gerenciamento, pode avançar
16. Execute o que foi definido e após isso em finish
17. Avance para outra tela
18. Deixe tudo padrão e finalize
19. Avance para outra tela
20. Essa tela será para testar a configuração, onde o usuário vai ser o root e a senha a que você escolheu, se funcionou, avance para outra tela
21. Execute e avançe
22. Desmarque a opção de executar shell e MySQL Workbench.

Obs: Não iremos executar o Workbench porque usaremos outro aplicativo para demonstrar sobre o SQL.

## **Linux**

No Linux, vamos instalar via terminal, seguindo pelos comando

```
$ sudo apt update
```
```
$ sudo apt install mysql-server
```
```
$sudo mysql_secure_installantion

Aqui pode dar 'N' para tudo por conta que vai ser somente um ambiente de desenvolvimento e onde você colocara sua senha.
```
```
$ mysql -u root -p
```
[Sub Conjuntos](../Introducao/Conjuntos.md) | [Inicio](../../README.md) | [Aplicativos](./Aplicativos.md)
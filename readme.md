# Projeto para estudo de SQL com MSSQL Server

Este projeto sobe um container com MSSQL Server instalado para estudar SQL para SQL SERVER. Versão do projeto é a 22.

## Referencia
### Container
[MSSQL Server container](https://hub.docker.com/r/microsoft/mssql-server)

### Estudos
[SQL Server 2022](https://learn.microsoft.com/pt-br/troubleshoot/sql/releases/download-and-install-latest-updates#sql-server-2022)

## IDE para SQL

Pode-se usar qualqu IDE para banco de dados
1. [SSMS](https://learn.microsoft.com/pt-br/ssms/install/install)
2. [DBeaver](https://dbeaver.io/download/)
3. [DataGrip](https://www.jetbrains.com/pt-br/datagrip/)

Ou pode ser qualquer IDE que dê suporte de alguma forma para conexão com MSSQL Server

## Docker com imagem SQL Server
### Dados de acesso
```
usuario: sa
senha: minhaSenhaForte#2026
```
### Porta

Porta padrão
```
1433
```

### Host
O host é o mesmo nome do serviço, neste caso
```
sqlserver
```
## Persistencia de dados

Caso queira manter a persistencia de dados, descomente as linhas do `docker-compose.yaml` referente a persistencia.

### Resetando a instalação

Desligue o container, remova tudo dentro da pasta de persistencia, comente as linhas novamente no arquivo `docker-compose.yaml` e inicie o container.
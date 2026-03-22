```bash
    docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=<password>" -e "MSSQL_PID=Express" -p 1433:1433 -d mcr.microsoft.com/mssql/server:2022-latest
```

```bash
    docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=<password>" -e "MSSQL_PID=Express" -p 1433:1433 -d mcr.microsoft.com/mssql/server:2019-latest
```

### permissions

```bash
    sudo mkdir ./<MSSQL_VOLUME_DATA>
    sudo chown -R 10001:0 ./<MSSQL_VOLUME_DATA>
    sudo chmod -R 770 ./<MSSQL_VOLUME_DATA>
```

##### MSSQL_USER=sa

#####

default user database

##### MSSQL_SA_PASSWORD=

#####

password user database

##### MSSQL_VOLUME_DATA=./mssql-data

#####

default volume folder

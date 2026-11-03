# Replication_Service_1

  CREATE USER monitor WITH PASSWORD 'Logicmo_2020';
  GRANT pg_monitor TO monitor;
ALTER USER monitor WITH PASSWORD 'Logicmo_2020';
host    postgres  monitor   192.168.1.100/32   scram-sha-256
# TYPE  DATABASE  USER      ADDRESS            METHOD
--add in booth svr 
host    postgres  postgres  192.168.1.100/32   scram-sha-256
host    postgres  monitor   192.168.1.100/32   scram-sha-256

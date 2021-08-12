# dockerhome
Files Needed to create docker based container home assistant and related services

# Influx 1.8
The following command are needed to set-up users in the database. 
CREATE DATABASE home_assistant
CREATE USER admin WITH PASSWORD 'ReplaceMe' WITH ALL PRIVILEGES
CREATE USER home_assistant WITH PASSWORD 'ReplaceMeToo'
GRANT READ on home_assistant TO home_assistant
GRANT WRITE on home_assistant TO home_assistant


In the influxdb.conf file
[http]
  enabled = true
  bind-address = ":8086"
  auth-enabled = true <- Change this to True
  log-enabled = true
  suppress-write-log = false
  write-tracing = false
  flux-enabled = false
  flux-log-enabled = false
  ... 

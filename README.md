# dockerhome
Files Needed to create docker based container home assistant and related services


CREATE DATABASE home_assistant
CREATE USER admin WITH PASSWORD 'ReplaceMe' WITH ALL PRIVILEGES
CREATE USER home_assistant WITH PASSWORD 'ReplaceMeToo'
GRANT READ on home_assistant TO home_assistant
GRANT WRITE on home_assistant TO home_assistant

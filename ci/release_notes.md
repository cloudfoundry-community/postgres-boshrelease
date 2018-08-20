# Improvements

Increase `monit start` timeout of the Postgres job to 60 seconds (previously 30
seconds). This fixes a bug where the Postgres job would be prematurely killed by
monit during boot.

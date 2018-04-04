# recovery_tests
Scripts for automating recovery tests.

When Barman server can not receive the version of the PostgreSQL server, it sets a string "FAILED" as a version number of PostgreSQL server. After a while the recovery script starts to compare the string "FAILED" with numbers. The script assumes that number is given as a version number, not a string and therefore fails to if the version number is not a number.

# groovy-cli-maven-mysql-function

## Description
Creates a small database table
called `dog`. This table, `dog`, has been normalized to 3NF.
Two new tables have been added, `breedLookup` and `colorLookup`.
Creates a new table `dog_expanded` that joins
`dog`, `breedLookup` and `colorLookup`. Added clustered indexes on
`dog`.breedId and `dog`.colorId and a non-clustered index for
`dog_expanded`.id. Turned `dog_expanded` into a view with an
implicit index on `dog_expanded`.id. Using an user defined function with the aggregate
COUNT, create a new view `breed_count`. All output normally
seen in a terminal will be in `groovy-srv/log` which will dump to the screen. The project may seem to hang but the logs from the container must be written to the project this can take up to 3 min.

## Tech stack
- groovy
- maven
  - log4j
  - mysql driver

## Docker stack
- maven:3-openjdk-17
- mariadb:latest

## To run
`sudo ./install.sh -u`
Creates groovy-srv/log

## To stop
`sudo ./install.sh -d`
Removes groovy-srv/log

## For help
`sudo ./install.sh -h`

## Credit
https://github.com/htorun/dbtableprinter

## groovy-cli specific search
- [Search by maven](https://github.com/bearddan2000?tab=repositories&q=groovy-cli-maven&type=&language=&sort=)
- [Search by mysql](https://github.com/bearddan2000?tab=repositories&q=groovy-cli-mysql&type=&language=&sort=)
- [Search by function](https://github.com/bearddan2000?tab=repositories&q=groovy-cli-function&type=&language=&sort=)
- [Search by log4j](https://github.com/bearddan2000?tab=repositories&q=groovy-cli-log4j&type=&language=&sort=)
- [Search by driver](https://github.com/bearddan2000?tab=repositories&q=groovy-cli-driver&type=&language=&sort=)

## General search
- [Search by groovy](https://github.com/bearddan2000?tab=repositories&q=java&type=&language=&sort=)
- [Search by cli](https://github.com/bearddan2000?tab=repositories&q=cli&type=&language=&sort=)
- [Search by maven](https://github.com/bearddan2000?tab=repositories&q=gradle&type=&language=&sort=)
- [Search by mysql](https://github.com/bearddan2000?tab=repositories&q=mysql&type=&language=&sort=)
- [Search by function](https://github.com/bearddan2000?tab=repositories&q=function&type=&language=&sort=)
- [Search by log4j](https://github.com/bearddan2000?tab=repositories&q=log4j&type=&language=&sort=)
- [Search by driver](https://github.com/bearddan2000?tab=repositories&q=driver&type=&language=&sort=)

# TODO: Notes to self

## Goals to remember
* Intuitive/easy to use
* Stand alone (no non-core dependencies)
* * Primary tool MUST remain a single file for ease of deployment
* Provide tools for BOTH parsing and analyzing (using both internal and external analysis tools)
* Support as many versions of perl as reasonably possible (while still staying 'modern')
* * Prefer a pseudo-object oriented style in keeping with 'modern' and 'standalone' objectives above
* Support as many versions of mysql as reasonably possible
* * Support as many versions of mysql slow query log as reasonably possible (e.g. Percona)
* Include some built in analysis tools for immediate use
* Facilitate easy integration with external analysis tools (gnuplot, R, etc)
* Use a sane set of defaults
* Document everything!

## Other similar projects of note
* https://github.com/jelder/slow_query_report
* https://github.com/LeeKemp/mysql-slow-query-log-parser
* http://www.retards.org/projects/mysql/
* http://www.mysqlperformanceblog.com/files/utils/mysql_slow_log_filter
* http://www.percona.com/doc/percona-toolkit/2.0/pt-query-digest.html
* http://www.percona.com/doc/percona-toolkit/2.0/pt-query-advisor.html


## TODO

* Add perldoc
* Add filter options (by user, by length, by host, by database, by table, by regex)
* Option to use perl grouping instead of mysqldumpslow grouping via regex (faster but less accurate)
* Option to track individual query over time (using string similarity) (how would you specify query??)
* Option to output as space/comma/tab delimited
* Option to include/exclude various output columns
* Verbose mode
* Option to turn off /tmp caching (requires either perl grouping or at least temporary file caching)
* Ambitious: html output (a la NYTProf??)
* Query analysis (perhaps via EXPLAIN or by detection of common pitfalls)
* Ambitious: output text bar graph of history (single query or all data)

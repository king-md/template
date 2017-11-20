# My getopt template - 

Source files here are for defining a standard launch point for any/all command line options for my code.  Specific ones for specific needs of various programs can always be done, but when needed command line parameters match ones in the getopt template, it is preferable to use these for sake of consistency between programs.

### Common Command Line Options

| Compiler        | Operating System             | Version String |
|-----------------|------------------------------|----------------|
| GCC 4.9.4       | Ubuntu 14.04.5 LTS           | g++-4.9 (Ubuntu 4.9.4-2ubuntu1~14.04.1) 4.9.4 |

| Option | Description | Notes |
| -a | all |  |
| -a | append |  |
| -b | buffer |  |
| -b | block |  |
| -b <#> | blocksize |  |
| -c <command string> | command to execute |  |
| -c <#> | count |  |
| -c | check |  |
| -c <filepath> | config file |  |
| -d | debug |  |
| -d | delete |  |
| -d <dir path> | directory |  |
| -e <exclusion string> | exclude |  |
| -e <execution string> | execute |  |
| -e <expression string> | expression |  |
| -f <filepath> | file |  |
| -f <email address> | from email address |  |
| -f | force |  |
| -g | reserved |  |
| -h | help (reserved by the argparse package) |  |
| -i <filepath> | input file |  |
| -i | interactive |  |
| -j | reserved |  |
| -k | keep |  |
| -l | long |  |
| -l | list |  |
| -l | login |  |
| -m <message string> | message |  |
| -n | no execute |  |
| -n <#> | number |  |
| -n | no or not |  |
| -o <filepath> | output file |  |
| -p <pw> | password |  |
| -p <#> | port |  |
| -p <string> | protocol |  |
| -q | quiet |  |
| -q <query string> | query |  |
| -r | recurse |  |
| -s | silent |  |
| -s <#> | size |  |
| -s <string> | string |  |
| -s <string> | subject |  |
| -t <time string> | time |  |
| -t <string> | type |  |
| -t <email address> | to email address |  |
| -u <id> | user |  |
| -v [<#>] | verbose, # is the verbosity level (default 1) [see also --verbose] |  |
| -w <#> | width |  |
| -x | debug |  |
| -x | exception |  |
| -x | extract |  |
| -y | yes |  |
| -z [<type>] | compression (type = [zip, gzip, Z] |  |
| -A | reserved |  |
| -B | reserved |  |
| -C | reserved |  |
| -D <key=value>[,<key=value>,...] | define |  |
| -E | reserved |  |
| -F | reserved |  |
| -G | reserved |  |
| -H | reserved |  |
| -I <include dir path> | include |  |
| -J | reserved |  |
| -K | reserved |  |
| -L | reserved |  |
| -M | reserved |  |
| -N | reserved |  |
| -O <order string> | order |  |
| -O <option string> | options |  |
| -P <#> | port number |  |
| -Q | reserved |  |
| -R | recurse |  |
| -S | stand alone |  |
| -T | reserved |  |
| -U | reserved |  |
| -V | version |  |
| -W | reserved |  |
| -X | reserved |  |
| -Y | reserved |  |
| -Z | reserved |  |
| -0 | reserved |  |
| -1 | reserved |  |
| -2 | reserved |  |
| -3 | reserved |  |
| -4 | reserved |  |
| -5 | reserved |  |
| -6 | reserved |  |
| -7 | reserved |  |
| -8 | reserved |  |
| -9 | reserved |  |
| --accept | accept |  |
| --accessed[=<datetime>] | accessed |  |
| --accessed-date[=<datetime>] | accessed-date |  |
| --after=<datetime> | after date of a date range |  |
| --after-date=<datetime> | after date of a date range |  |
| --alarm=<datetime> | alarm time |  |
| --alias=<key=value>[,<key=value>,...] | alias key=value |  |
| --all | process all elements |  |
| --append | append |  |
| --archive=<dirpath> | archive dir path |  |
| --archive-name=<dirpath> | archive dir path |  |
| --ascii | ASCII |  |
| --avoid-wraps | avoid-wraps |  |
| --background | execute in the background |  |
| --backup=<dirpath> | backup the data/config |  |
| --backups | backups |  |
| --backward-search | search in reverse order |  |
| --basename | basename |  |
| --batch | execute in batch mode (not interactive) |  |
| --baud=<speed value> | set the communication speed |  |
| --before=<datetime> | before date of a date range |  |
| --before-date=<datetime> | before date of a date range |  |
| --binary | binary mode (not text mode) |  |
| --block-size=<size> | block-size |  |
| --blocks | blocks |  |
| --brief | display minimal output |  |
| --buffer | buffer |  |
| --bytes | bytes |  |
| --cache | cache |  |
| --catenate | catenate |  |
| --cd=<dirpath> | set working directory |  |
| --changes | changes |  |
| --character-count | character-count |  |
| --check | check |  |
| --check-existing | check-existing |  |
| --child | child |  |
| --classify | classify |  |
| --clean | clean |  |
| --clear | clear |  |
| --close | close |  |
| --colons | colons |  |
| --column=<#|string> | column |  |
| --command=<command string> | command to execute |  |
| --common | common |  |
| --compare | compare |  |
| --compress[=<type>] | compress using the specified type of compression |  |
| --compression[=<type>] | compression (type = [zip, gzip, Z] |  |
| --concatenate | concatenate |  |
| --connect | connect |  |
| --copy | copy |  |
| --core | core |  |
| --count | count |  |
| --create | create |  |
| --created[=<datetime>] | created |  |
| --created-date[=<datetime>] | created-date |  |
| --date=<datetime> | date |  |
| --date-time=<datetime> | date-time |  |
| --date-time-stamp=<datetime> | date-time-stamp |  |
| --debug | debug |  |
| --decrypt[=<type>] | decrypt using specified type of encryption |  |
| --default | default |  |
| --define=<key=value>[,<key=value>,...] | define |  |
| --delete | delete |  |
| --delimeter=<value> | delimeter |  |
| --description=<string> | description |  |
| --device=<device ref> | device |  |
| --diff | diff |  |
| --digits | digits |  |
| --directory=<dirpath> | directory |  |
| --disable=<key>[,<key>,...] | disable |  |
| --discard-all | discard-all |  |
| --discard-locals | discard-locals |  |
| --disconnect | disconnect |  |
| --domain=<name string> | domain |  |
| --domain-name=<name string> | domain-name |  |
| --dry-run | dry-run |  |
| --elapsed | elapsed |  |
| --enable=<key>[,<key>,...] | enable |  |
| --encode=<type> | encode |  |
| --encoding=<type> | encoding |  |
| --encrypt[=<type>] | encrypt using specified type of encryption |  |
| --environment-overrides=<key=value>[,<key=value>,...] | environment-overrides |  |
| --eof | eof |  |
| --epoch=<value> | epoch |  |
| --erase | erase |  |
| --error-limit[=<value>] | error-limit |  |
| --error-output | error-output |  |
| --escape | escape |  |
| --event | event |  |
| --event-id=<#|string>- event-id |  |
| --event-name<string> | event-name |  |
| --exclude | exclude |  |
| --exclude-from | exclude-from |  |
| --exec=<execute string> | exec |  |
| --exit | exit |  |
| --expand-tabs | expand-tabs |  |
| --export=<filepath> | export |  |
| --expression=<expression string> | expression |  |
| --extract | extract |  |
| --fast | fast |  |
| --fatal-warnings | fatal-warnings |  |
| --fetch=<fetch string> | fetch |  |
| --field-separator=<field seperator char> | field-separator |  |
| --file=<filepath> | file |  |
| --file-prefix=<prefix string> | file-prefix |  |
| --file-suffix=<suffix string> | file-suffix |  |
| --file-type=<type> | file-type |  |
| --filter | filter |  |
| --fix | fix |  |
| --flag | flag |  |
| --follow | follow |  |
| --force | force |  |
| --force-prefix=<prefix string> | force-prefix |  |
| --foreground | foreground |  |
| --format=<format string> | format |  |
| --fqdn=<domain name> | fqdn |  |
| --frequency=<freq value> | frequency |  |
| --from=<email address> | from email address |  |
| --fully-qualified-domain-name=<domain name> | fully qualified domain name |  |
| --get | get |  |
| --graphic | graphic |  |
| --group=<group #|group name> | group |  |
| --guid=<guid #> | guid |  |
| --hashsize=<size> | hashsize |  |
| --header=<key=value>[,<key=value>,...] | header |  |
| --heading | heading |  |
| --history | history |  |
| --host=<hostname> | host |  |
| --host-name=<hostname> | host-name |  |
| --html | html |  |
| --id=<#> | id |  |
| --idle | idle |  |
| --ignore | ignore |  |
| --ignore-all-newlines | ignore-all-newlines |  |
| --ignore-all-space | ignore-all-space |  |
| --ignore-all-tabs | ignore-all-tabs |  |
| --ignore-all-whitespace | ignore-all-whitespace |  |
| --ignore-blank-lines | ignore-blank-lines |  |
| --ignore-case | ignore-case |  |
| --ignore-errors | ignore-errors |  |
| --ignore-file=<filepath> | ignore-file |  |
| --ignore-indentation | ignore-indentation |  |
| --ignore-interrupts[=<#|name>[,<#|name>,...]] | ignore-interrupts |  |
| --ignore-matching-lines | ignore-matching-lines |  |
| --ignore-null | ignore-null |  |
| --ignore-zeros | ignore-zeros |  |
| --import=<filepath> | import |  |
| --include=<filepath> | include |  |
| --include-dir=<dirpath> | include-dir |  |
| --increment | increment |  |
| --incremental | incremental |  |
| --info | info |  |
| --init-file=<filepath> | init-file |  |
| --initial | initial |  |
| --initial-tab | initial-tab |  |
| --initialize | initialize |  |
| --input-file=<filepath> | input file |  |
| --insert | insert |  |
| --install | install |  |
| --interactive | interactive |  |
| --interface=<iface name> | interface |  |
| --interface-name=<iface name> | interface-name |  |
| --interval=<#> | interval |  |
| --ip=<ip addr> | ip |  |
| --ipaddr=<ip addr> | ipaddr |  |
| --ip-address=<ip addr> | ip-address |  |
| --job=<#|name> | job |  |
| --job-id=<#> | job-id |  |
| --job-name=<name> | job-name |  |
| --json | json |  |
| --just-print | just-print |  |
| --keep[=<string>] | keep |  |
| --keep-going | keep-going |  |
| --keep-files=<filepath>[,<filepath>,...] | keep-files |  |
| --kilobytes | kilobytes |  |
| --language=<lang identifier> | language |  |
| --length=<#> | length |  |
| --level=<#> | level |  |
| --limit=<#> | limit |  |
| --line[=<#>] | line |  |
| --line-bytes | line-bytes |  |
| --list | list |  |
| --lock | lock |  |
| --log[=<filepath>] | log |  |
| --log-dir=<dirpath> | log-dir |  |
| --log-dir-path=<dirpath> | log-dir-path |  |
| --log-level=<#|level name> | log-level |  |
| --log-path=<dirpath> | log-path |  |
| --log-roll[=<frequency>] | log-roll |  |
| --log-type=<type> | log-type |  |
| --login | login |  |
| --long | long |  |
| --lower | lower |  |
| --lower-case | lower-case |  |
| --mac=<mac addr> | mac |  |
| --macaddr=<mac addr> | macaddr |  |
| --mac-address=<mac addr> | mac-address |  |
| --machine=<machine identifier> | machine |  |
| --macro=<key=value>[,<key=value>,...] | macro |  |
| --macro-name=<key=value>[,<key=value>,...] | macro-name |  |
| --mail | mail |  |
| --make-directories[=<dirpath>[,<dirpath>,...]] | make-directories |  |
| --makefile=<filepath> | makefile |  |
| --map | map |  |
| --mapped | mapped |  |
| --mask=<mask value> | mask |  |
| --matching | matching |  |
| --matching-lines | matching-lines |  |
| --max[=<value>] | max |  |
| --max-args | max-args |  |
| --max-chars | max-chars |  |
| --max-lines | max-lines |  |
| --max-load[=<value>] | max-load |  |
| --max-procs | max-procs |  |
| --mesg=<string> | mesg |  |
| --message=<string> | message |  |
| --min[=<value>] | min |  |
| --minimal | minimal |  |
| --mode[=<value>] | mode |  |
| --modified | modified |  |
| --modified-date[=<date string>] | modified-date |  |
| --modify | modify |  |
| --modification-time[=<datetime>] | modification-time |  |
| --move | move |  |
| --name=<string> | name |  |
| --name-prefix=<string> | name-prefix |  |
| --name-suffix=<string> | name-suffix |  |
| --nesting-limit=<#> | nesting-limit |  |
| --net | net |  |
| --net-headers | net-headers |  |
| --new | new |  |
| --new-file=<filepath> | new-file |  |
| --no-character-count | no-character-count |  |
| --no-check | no-check |  |
| --no-check-existing | no-check-existing |  |
| --no-common | no-common |  |
| --no-create | no-create |  |
| --no-execute | no-execute |  |
| --no-backups | no-backups |  |
| --no-init-file | no-init-file |  |
| --no-keep-going | no-keep-going |  |
| --no-lines | no-lines |  |
| --no-prof | no-prof |  |
| --no-profile | no-profile |  |
| --no-regex | no-regex |  |
| --no-sort | no-sort |  |
| --no-time | no-time |  |
| --no-timestamp | no-timestamp |  |
| --no-validate | no-validate |  |
| --no-wait | no-wait |  |
| --no-warn | no-warn |  |
| --node=<node name> | node |  |
| --nodename=<node name> | nodename |  |
| --nonmatching | nonmatching |  |
| --notify | notify |  |
| --null | null |  |
| --number[=<#>] | number |  |
| --old-archive=<dirpath> | old-archive |  |
| --old-file=<filepath> | old-file |  |
| --options=<key=value>[,<key=value>,...] | options |  |
| --other | other |  |
| --output[=<filepath>] | output |  |
| --output-file=<filepath> | output file |  |
| --output-prefix=<string> | output-prefix |  |
| --output-suffix=<string> | output-suffix |  |
| --override | override |  |
| --overwrite | overwrite |  |
| --own[=<#|name>] | own |  |
| --owner[=<#|name>] | owner |  |
| --open[=<filepath>] | open |  |
| --paginate | paginate |  |
| --paragraph-indent | paragraph-indent |  |
| --parent | parent |  |
| --parents | parents |  |
| --pid=<#> | pid |  |
| --ping[=<ipaddr|string>] | ping |  |
| --pop | pop |  |
| --port=<#|name> | port |  |
| --port-name=<name> | port-name |  |
| --ppid=<#> | ppid |  |
| --prefix=<string> | prefix |  |
| --preserve | preserve |  |
| --preserve-environment | preserve-environment |  |
| --preserve-modification-time | preserve-modification-time |  |
| --preserve-order | preserve-order |  |
| --preserve-permissions | preserve-permissions |  |
| --pri=<#|string> | pri |  |
| --print | print |  |
| --print-data-base | print-data-base |  |
| --print-directory | print-directory |  |
| --print-file-name | print-file-name |  |
| --print-symdefs | print-symdefs |  |
| --printer=<print identifier> | printer |  |
| --priority=<#|string> | priority |  |
| --prof | prof |  |
| --profile | profile |  |
| --prompt=<string> | prompt |  |
| --proxy=<proxy string> | proxy |  |
| --purge | purge |  |
| --push | push |  |
| --query=<query string> | query |  |
| --query-user=<user id> | query-user |  |
| --question=<string> | question |  |
| --quiet | quiet |  |
| --quote=<string> | quote |  |
| --quote-name=<string> | quote-name |  |
| --read | read |  |
| --read-full | read-full |  |
| --read-full-blocks | read-full-blocks |  |
| --read-now | read-now |  |
| --read-only | read-only |  |
| --read-write | read-write |  |
| --receive | receive |  |
| --record[=<#|identifier>] | record |  |
| --record-number=<#> | record-number |  |
| --recursive | recursive |  |
| --reference | reference |  |
| --regex=<regex string> | regex |  |
| --reject | reject |  |
| --release | release |  |
| --reload | reload |  |
| --reload-state | reload-state |  |
| --relocation | relocation |  |
| --remove=<string> | remove |  |
| --rename=<old string=new string> | rename |  |
| --repair | repair |  |
| --repeat | repeat |  |
| --replace=<old string=new string> | replace |  |
| --report | report |  |
| --report-identical | report-identical |  |
| --report-identical-files | report-identical-files |  |
| --reset | reset |  |
| --reset-access-time | reset-access-time |  |
| --resolve | resolve |  |
| --restart | restart |  |
| --restore | restore |  |
| --resume | resume |  |
| --retry | retry |  |
| --reverse | reverse |  |
| --role=<role identifier> | role |  |
| --save | save |  |
| --send | send |  |
| --separator=<seperator char> | separator |  |
| --sequence | sequence |  |
| --set | set |  |
| --sgml | sgml |  |
| --shell=<shell name> | shell |  |
| --show | show |  |
| --show-all | show-all |  |
| --show-tabs | show-tabs |  |
| --silent | silent |  |
| --size=<#> | size |  |
| --socket=<socket identifier> | socket |  |
| --sort | sort |  |
| --sort-alpha | sort-alpha |  |
| --sort-alphanumeric | sort-alphanumeric |  |
| --sort-binary | sort-binary |  |
| --sort-hexidecimal | sort-hexidecimal |  |
| --sort-numeric | sort-numeric |  |
| --sort-octal | sort-octal |  |
| --source=<string> | source |  |
| --sparse | sparse |  |
| --speed=<#> | speed |  |
| --split | split |  |
| --split-size-limit=<#> | split-size-limit |  |
| --squeeze-blank | squeeze-blank |  |
| --start | start |  |
| --state=<state identifier> | state |  |
| --statistics | statistics |  |
| --strict | strict |  |
| --strip | strip |  |
| --strip-all | strip-all |  |
| --stop | stop |  |
| --submitter=<string> | submitter |  |
| --suffix=<string> | suffix |  |
| --sum | sum |  |
| --summarize | summarize |  |
| --suspend | suspend |  |
| --symbolic | symbolic |  |
| --symbols=<key=value>[,<key=value>,...] | symbols |  |
| --syslog[=<filepath>] | syslog |  |
| --tabs | tabs |  |
| --tabsize=<#> | tabsize |  |
| --target=<string> | target |  |
| --temp=<filepath> | temp |  |
| --tempdir=<dirpath> | tempdir |  |
| --temporary=<filepath> | temporary |  |
| --temporary-directory=<dirpath> | temporary-directory |  |
| --terminal=<type> | terminal |  |
| --test | test |  |
| --text | text |  |
| --time=<timestamp> | time |  |
| --timeout=<timestamp> | timeout |  |
| --timer=<timestamp> | timer |  |
| --timestamp=<timestamp> | timestamp |  |
| --to=<email address> | to email address |  |
| --total | total |  |
| --touch | touch |  |
| --trace | trace |  |
| --truncate | truncate |  |
| --type=<type> | type |  |
| --uid=<#> | uid |  |
| --unblock | unblock |  |
| --uncompress[=<compression type>] | uncompress using the specified type of compression |  |
| --unconditional | unconditional |  |
| --undefine=<identifier>[,<identifier>,...] | undefine |  |
| --undefined-only | undefined-only |  |
| --uninstall | uninstall |  |
| --unique | unique |  |
| --unlock | unlock |  |
| --unset=<identifier>[,<identifier>,...] | unset |  |
| --update | update |  |
| --upper | upper |  |
| --upper-case | upper-case |  |
| --uri=<uri string> | uri |  |
| --url=<url string> | url |  |
| --usage | usage |  |
| --user=<#|name> | user |  |
| --username=<name> | username |  |
| --user-name=<name> | user-name |  |
| --validate | validate |  |
| --verbose[=<#>] | verbose, # is the verbosity level (default 1) [see also --v] |  |
| --verify | verify |  |
| --version | version |  |
| --version-control | version-control |  |
| --volume=<value> | volume |  |
| --wait[=<wait time>] | wait |  |
| --warn | warn |  |
| --width=<#> | width |  |
| --wrap[=<#>] | wrap |  |
| --write | write |  |
| --writable | writable |  |
| --xml | xml |  |
| --zeros | zeros |  |

### Languages with a getopt template file:

| Language | Filename | Notes |
| Python3 | getopt_template.py | work in progress |
| C | TBD | future goal |
| C++ | TBD | future goal |
| C# | TBD | future goal |
| node.js | TBD | future goal |
| bash | TBD | future goal |
| GO | TBD | future goal |
| Java | TBD | future goal |

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Prerequisites/requirements vary for each languange.

| Language | Required | Notes |
| Python3 | import argparse | - |
| C | TBD | - |
| C++ | TBD | - |
| C# | TBD | - |
| node.js | TBD | - |
| bash | TBD | - |
| GO | TBD | - |
| Java | TBD | - |

### Installing

Get a copy of the template/getopt repository.

```
git clone https://github.com/king-md/template.git
```

Copy the template/getopt/getopt_template.\* file to the directory where you want to work with it.

```
Windows: copy template\getopt\getopt_template.\* C:\DESTINATION

Linux: cp -p template/getopt/getopt_template.\* /home/user/bin/.
```

## Contributing

Not available at this time.

## Versioning

Not available at this time.

## Authors

* **Michael King** - *Initial work* - 

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

Not available at this time.


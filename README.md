## Ansible Play➜Doc

Creates human-readable instructions from [Ansible](https://ansible.com) Playbooks.

Output formats:
* Wiki
* Markdown

### Usage
```
playtodoc [-h] [--version] [-b BASEDIR] [-f FORMAT] [-o FILENAME] [-l LIMIT] [-v] playbook.yml

Convert Ansible Playbooks to various Markup format for human consumption.

positional arguments:
  playbook.yml

optional arguments:
  -h, --help            show this help message and exit
  --version             show program's version number and exit
  -b BASEDIR, --basedir BASEDIR
                        Ansible base dir for playbooks, roles, vars, etc.
  -f FORMAT, --format FORMAT
                        Output format, can be one of 'md', 'wiki'
  -o FILENAME, --output FILENAME
                        Output filename
  -l LIMIT, --limit LIMIT
                        Template and file inline character limit. Rendered
                        templates and files longer than this will be printed
                        into separate files and linked to. Defaults to 1000.
  -v, --verbose         Be more verbose
```

### Status

alpha, very rudimentary output.

Todo:
* more modules
* proper `with_*`-support
* more output formats

Not-Todo:
* all modules
* support for weird configurations and deep magic - standard playbooks & roles only

# Ansible role for prometheus-postgres-exporter

This Ansible role installs the `prometheus-postgres-exporter` on Debian-based
systems. It assumes that PostgreSQL is running on the same host that the role
is running on, and automatically creates a `prometheus` user used for any
monitoring queries.

## Installation

To install, add the following to your `requirements.yml`:

```yaml
roles:
  - src: https://github.com/jchristgit/ansible-role-prometheus-postgres-exporter
    scm: git
    version: master
    name: prometheus-postgres-exporter
```

## Requirements

The `libpq-dev` and `python3-psycopg2` packages should be installed on your
host already for the Ansible PostgreSQL management modules to work properly.


<!-- vim: set textwidth=80 sw=2 ts=2: -->

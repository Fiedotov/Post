# README

# Installing Pigsty

We want to use [Rocky Linux 8.8](https://wiki.rockylinux.org/rocky/version/), per their recommendation:

![rocky](./docs/images/rocky.png)

## Install steps:

- `yum update -y`
- `yum install tar -y`
- `dnf install epel-release -y` (thanks to [Pigsty (Ercan)](https://www.notion.so/Pigsty-Ercan-f7f47bdb72b6478790ca5f58ffd6e011?pvs=21))
- `dnf upgrade -y -v`
- `wget http:[//github.com/Vonng/pigsty/releases/download/v2.5.0/pigsty-pkg-v2.5.0.el8.x86_64.tgz](notion://github.com/Vonng/pigsty/releases/download/v2.5.0/pigsty-pkg-v2.5.0.el8.x86_64.tgz)`
- `mv pigsty-pkg-v2.5.0.el8.x86_64.tgz /tmp/pkg.tgz`

**Notes**:

using the latest (2.5.0) from Github, as the website doesn’t appear to be updated: https://github.com/Vonng/pigsty

# Questions on Pigsty

See issue: https://github.com/BuildRemote/stackgres-to-pigsty/issues/1

## How to run single vs. multi-node

## How do you install extensions?

Test the installation of these extensions and explain how it’s done, step by step. (then remove this line from the README)

### timescale

### pg_trgm

### pgvector

## See if Grafana dashboard shows slow queries. Include a screenshot.

Yes, very much.

![slow-queries](./docs/images/slow-queries.png)

## Run backup and restore

Use remote storage, not local minio

Also curious how much performance impact a backup has. Is incremental backup supported?

## Major and minor version upgrades

Does minor and major version upgrade work as described?

## Major upgrade

### Upgrading from version X to version Y

### Downgrading from Y to X

## Minor upgrade

### Upgrading from version X.01 to X.02

## Downgrading from version X.02 to X.01

## Setting connection pool sizes

How to set different connection pool size for different users

## Read-only replicas

How to add read only replica and connect to it

## Alerts

How to get alerts about connection pool running out of connections

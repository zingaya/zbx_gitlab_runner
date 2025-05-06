# Zabbix Gitlab runner
## Overview

A simple Zabbix template to monitor Gitlab runners.

## Usage

Make sure you have enabled and Zabbix server/proxy can reach the runner.
You have to add/modify this line in the `/etc/gitlab-runner/config.toml`

    listen_address = "IP:PORT"

Then add this Zabbix template to the host, and adjust both macros as needed:\

`{$GITLABRUNNER.METRICS.HOST}`\
`{$GITLABRUNNER.METRICS.PORT}`

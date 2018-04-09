# fluent

simple cookbook for managing td-agent{,-bit} (fluent{d,bit})

## recipes

- default: install, configure, manage td-agent

- fluentd: install, configure, manage td-agent
- fluent_bit: install, configure, manage td-agent-bit

- fluentd_install: install td-agent
- fluentd_configure: configure td-agent debug input, set up include dir
- fluentd_manage: manage td-agent service

- fluent_bit_install: install td-agent-bit
- fluent_bit_configure: configure td-agent-bit, set up include mgmt
- fluent_bit_manage: manage td-agent-bit service

## resources

### fluentd\_cfg

a light wrapper around the file resource that sets up a default install path of `/etc/td-agent/conf.d/#{name}.conf`

### fluent\_bit\_cfg

a light wrapper around the the file resource that sets up a default install path of `/etc/td-agent-bit/conf.d/#{name}.conf`

### fluentd\_gem

a light wrapper around the gem_package resource that sets the default gem_binary to `/sbin/td-agent-gem`

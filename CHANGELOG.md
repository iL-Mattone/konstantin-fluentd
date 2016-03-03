## Unreleased

## 2016-03-03 - Release Branch feature/ruby1.8.7 

 - params.pp : for backward compatibility with ruby 1.8.7 seems to work better when moving the conditional check for serviceprovider ( https://tickets.puppetlabs.com/browse/PUP-5296 ) into the osfamily catch block.
 - install_repo.pp : added a conditional if-block if we dont want to specify ( or cant use for whatever reason ) the gpgkey for the case of redhat/centos rpms.   

## 2016-01-22 - Release v. 0.3.2

 - Purge unmanaged config files
 - Manage td-agent.conf file with a fully qualified path
 - Fix the issue with td-agent service being enabled on each run on EL7

## 2015-12-02 - Release v. 0.3.1

 - Add param `repo_desc`

## 2015-10-28 - Release v. 0.3.0

 - Remove class `fluentd::config`
 - Add defined type `fluentd::config`
 - Add defined type `fluentd::plugin`

## 2015-10-22 - Release v. 0.2.0

 - Add param `service_manage`
 - Add param `repo_gpgkeyid`
 - Add param `repo_install`
 - Add param `plugin_source`
 - Rename param `repo_baseurl` to `repo_url`
 - Remove param `config_template`
 - Param validation
 - Support Ubuntu 14.04
 - Support Debian 7.8
 - Support nested config tags

## 2015-10-19 - Release v. 0.1.0

 - Initial release

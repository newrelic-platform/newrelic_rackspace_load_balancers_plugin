# Rackspace Load Balancers plugin

## Dependencies/Requirements
* Ruby (>= 1.8.7)
* Rubygems (>= 1.3.7)
* Bundler `gem install bundler`
* Logging must be enabled on the load balancer nodes.

## First Time Setup Instructions
1. Download the latest tagged version from [HERE](https://github.com/newrelic-platform/newrelic_rackspace_load_balancers_plugin/tags)
2. Extract to the location you want to run the plugin from
3. Run `bundle install --binstubs`
4. Run `./bin/newrelic_rs --sample-config`
5. Edit `config/newrelic_plugin.yml` (See configuration information section for additional information)

## Configuration Information
1. Replace 'LICENSE KEY' with your New Relic license key
2. Replace 'USERNAME' with your Rackspace username
3. Replace 'KEY' with your Rackspace API key. This can be found under API Keys in your Rackspace account settings.
4. Replace 'REGION' with the region your load balancer is located. This should be 'ord' or 'dfw'. ( *Note:* This is case sensitive)

###Special Instructions for use with multiple regions
If your load balancers are in multiple regions, copy all files to a secondary directory and modify the configuration files to reflect the secondary region. You will need to run the agent twice, once for each region.

## Running the agent

To start the agent run: `./bin/newrelic_rs`

## Keep this process running
You can use services like these to manage this process. 
- [Upstart](http://upstart.ubuntu.com/)
- [Systemd](http://www.freedesktop.org/wiki/Software/systemd/)
- [Runit](http://smarden.org/runit/)
- [Monit](http://mmonit.com/monit/)

## For Support
Plugin support and troubleshooting assistance can be obtained by visiting [support.newrelic.com](https://support.newrelic.com)

## Credits
The New Relic Rackspace Load Balancers plugin was originally authored by [Sean Porter](https://github.com/portertech) and the team at [Heavy Water Operations](http://hw-ops.com/). Subsequent updates and support are provided by [New Relic](http://newrelic.com/platform).

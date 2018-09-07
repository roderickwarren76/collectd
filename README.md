# collectd
Template used for Collectd and Couchdb 2.2.0

To use this config file, there are a few things that will need to be done.

1. Install Collectd (please check the collectd wiki for instructions)
2. Edit config file with the hostname of the machine that will be used
3. Edit the network plugin with the networking details of the system that will store the metrics. In this case, InfluxDB is used.
4. Edit the config file for the couch objects that are needed. Keep in mind, that the more objects you read, the possibilty will occur, where the read threads for collectd will need to be increased. (please check the collectd wiki for instructions)
5. Copy over the new config file to the machine that collectd was installed on.
6. Copy over the additional Typesdb file to the machine that collectd was installed on, and the database server that is capturing the data. In this case, InfluxDB is used. Please consult the Influxdb documentation for more information.
7. Restart Collectd with the new config.

Some additional changes to the config file may be warrented, due to the config being written for a x64 CentOS machine. Please consult the collectd wiki for more information.


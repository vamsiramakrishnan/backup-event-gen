# backup-event-gen
A Function that sends payload from Notifications to Splunk . 

Configure parameters as follows

| Fn-Name               | Parameter Name     | Description                                                                                                   | Example                                   |
| --------------------- | ------------------ | ------------------------------------------------------------------------------------------------------------- | ----------------------------------------- |
| splunk-export-payload | source_source_name | The Source Name that you would like Splunk to see                                                             | oci-hec-event-collector                   |
| splunk-export-payload | source_host_name   | The Source Hostname that you would like Splunk to see                                                         | oci-audit-logs                            |
| splunk-export-payload | splunk_url         | The Splunk Cloud URL ( Append input to the beginning of your splunk cloud url, do not add any http/https etc. | input-prd-p-hh6835czm4rp.cloud.splunk.com |
| splunk-export-payload | splunk_hec_token   | The Token that is unqiue to that HEC                                                                          | TOKEN                                     |
| splunk-export-payload | splunk_index_name  | The index into which you'd like these logs to get aggregated                                                  | main                                      |
| splunk-export-payload | splunk_hec_port    | The listener port of the HEC Endpoint of Splunk                                                               | 8088                                      |
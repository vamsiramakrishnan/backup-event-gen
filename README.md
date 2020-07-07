# backup-event-gen
A Function that sends payload from Notifications to Splunk . 

Configure parameters as follows

| Fn-Name           | Parameter Name     | Description                                                                                                   | Example                                   |
| ----------------- | ------------------ | ------------------------------------------------------------------------------------------------------------- | ----------------------------------------- |
| publish-to-splunk | source_source_name | The Source Name that you would like Splunk to see                                                             | oci-hec-event-collector                   |
| publish-to-splunk | source_host_name   | The Source Hostname that you would like Splunk to see                                                         | oci-audit-logs                            |
| publish-to-splunk | splunk_url         | The Splunk Cloud URL ( Append input to the beginning of your splunk cloud url, do not add any http/https etc. | input-prd-p-hh6835czm4rp.cloud.splunk.com |
| publish-to-splunk | splunk_hec_token   | The Token that is unqiue to that HEC                                                                          | TOKEN                                     |
| publish-to-splunk | splunk_index_name  | The index into which you'd like these logs to get aggregated                                                  | main                                      |
| publish-to-splunk | splunk_hec_port    | The listener port of the HEC Endpoint of Splunk                                                               | 8088                                      |
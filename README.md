cli-utils-in-perl
=================
Some handy command line utils written in perl.


multicores_exporter_4solr
-------------------------
1. Divide all solr cores to groups according to cores and times(how many times needed to complete on all groups,there are one or more cores inside a group).

2. Construct query line and shards line,set result format as "csv".

3. Query solr multi cores by using solr provided "shards" parameter,fire request with `curl`.

4. Get result one group by one group and append result to a single file.


sftp file fetcher and processer and uploader
--------------------------------------------
Both the fetcher and processer can accept argument or STDIN,so it can be used in shell pipeline.

###Example:
>sftp_transfer  -f|file_processor|sftp_transfer -u

###There are Net::SSH2 version and pure version(without any external dependency).

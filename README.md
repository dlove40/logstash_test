# logstash_test
Install and configure logstash
Input
The LogStash configuration file is set to monitor for input from the CLI that started the logstash.bat file, log files in a defined path, and logs sent to TCP port 5000. 
Filters
The filters in the configuration are determined by the input type. Custom patterns were created to extract the desired information from the logs. Duplicate and irrelevant fields have been removed to help make the data more presentable.  Severity numeric data will be replaced with a corresponding severity level after the data has been parsed.
Output
The data will be output into two formats. A CSV file that will include columns for the relevant data, and a text file containing the data in a json format.

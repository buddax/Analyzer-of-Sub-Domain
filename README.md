The "SubDomain Analyzer" tool written in Python language. The purpose of "SubDomain Analyzer" getting full detailed information of selected domain. The "SubDomain Analyzer" gets data from domain by following steps:

    Trying to get the zone tranfer file.
    Gathers all information from DNS records.
    Analyzing the DNS records (Analyzing all IP's addresses from DNS records and test class C range from IP address (For example: 127.0.0.1/24) and getting all data that containing the domain being analyzed).
    Tests subdomains by dictionary attack.

The Subdomain Analyzer can keep new addresses which found on DNS records or IP's analyzer. The Subdomain Analyzer can brings a very qualitative information about the domain being analyzed, additionally, he shows a designed report with all the data.
Examples:

    Analyzing example.com domain: subdomain-analyzer.py example.com
    Analyzing example.com domain, save the records on log file by name log.txt, works with 100 threads and use by another dictionary file by name another-file.txt: subdomain-analyzer.py example.com --output log.txt --threads 100 --sub-domain-list another-file.txt
    Analyzing example.com domain, save the records on log file by name log.txt and append a new sub-domains to sub-domains list file: subdomain-analyzer.py example.com -o log.txt --sub-domain-list


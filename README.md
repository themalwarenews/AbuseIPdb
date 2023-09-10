
# AbuseIPdb

This script is designed to streamline the process of scanning a list of IP addresses from AbuseIPDB and extracting valuable information. It then organizes this data into a CSV file. This tool is incredibly useful for threat hunting and improving incident response times in cybersecurity.

![image](https://github.com/themalwarenews/AbuseIPdb/assets/31186224/a4d2e410-6535-4850-870d-ebe903a0cb36)


## Installation

Install AbuseIPdb with `git`

```bash
 git clone https://github.com/themalwarenews/AbuseIPdb
 cd AbuseIPdb
 pip3 install -r requirements.txt
 python3 AbuseIPdb.py <flag> <arguments>
```
    
## Usage

```bash
 python3 AbuseIPdb.py -h

usage: abuse.py [-h] [-f FILE | -i IP | -b BLOCK | -cc COUNTRYCODE]
                [-c CSV | -j JSON | -l JSONL | -t TSV] [-d DAYS] [-x] [-v]

This program utilizes the Abuse IP Database from: AbuseIPDB.com to perform queries about IP
addresses and returns the output to standard out.

options:
  -h, --help            show this help message and exit
  -f FILE, --file FILE  parses IP Addresses from a single given file
  -i IP, --ip IP        lookup a single IP address
  -b BLOCK, --block BLOCK
                        lookup an IP block
  -cc COUNTRYCODE, --countrycode COUNTRYCODE
                        Select a country code to check IP range
  -c CSV, --csv CSV     outputs items in comma seperated values
  -j JSON, --json JSON  outputs items in json format (reccomended)
  -l JSONL, --jsonl JSONL
                        outputs items in jsonl format (reccomended
  -t TSV, --tsv TSV     outputs items in tab seperated values (Default)
  -d DAYS, --days DAYS  take in the number of days in history to go back for IP reports.
                        Default: 30 Days
  -x, --translate       By default categories are numbers, with this flag it will convert them
                        to text
  -v, --version         show program version
```

### Scan a Single IP
``` bash
python3 AbuseIPdb.py -i 1.1.1.1 

```

### Scan a Multiple IP and output to CSV
``` bash
python3 AbuseIPdb.py -f IPlist.txt -c output.csv

```

### Scan a Multiple IP and output to JSON
``` bash
python3 AbuseIPdb.py -f IPlist.txt -j output.json

```
### Example 


https://github.com/themalwarenews/AbuseIPdb/assets/31186224/47265b29-5d7a-4c5a-9a76-65887f427dda


  Feel free to notify us for any errors :slightly_smiling_face:
  
  Follow us on :

[<img src='https://user-images.githubusercontent.com/100226024/229274315-c12a320c-cf5b-44da-ae6d-f3811957663d.svg' alt='linkedin' height='40'>](https://www.linkedin.com/in/anonsharan/) 	 [<img src='https://user-images.githubusercontent.com/100226024/229274268-453d1eec-4d98-4dad-80c8-885b4c6d0854.svg' alt='instagram' height='40'>](https://www.instagram.com/hackwithsharan/)  [<img src='https://user-images.githubusercontent.com/100226024/229274348-8af09e55-c563-4e0c-9118-59af0fda9df9.svg' alt='twitter' height='40'>](https://twitter.com/anon_sharzzk)  [<img src='https://user-images.githubusercontent.com/100226024/229274377-07f7c7d2-2cf9-4bfc-8727-0eba0eb4cfe4.svg' alt='YouTube' height='40'>](https://www.youtube.com/channel/ByteTheories)








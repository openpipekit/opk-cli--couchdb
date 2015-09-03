# OPK CLI: CouchDB command line interface for Open Pipe Kit  
A commandline interface for pushing data into CouchDB. You can pipe a single value to this CLI or JSON. You can also pipe a stream of data to this CLI where each new line is a new value. The CLI will exit when it hears an exit code from the left side of the pipe. 

```
./push
  --username [account] Example: jansmith
  --password [password] Example: foobar
  --database <database name> Example: my_sensortag
  --url <couchdb url> Example: janesmith.cloudant.com
  --noTimestamp Prevent a timestamp from being added to your data
  --verbose Use for debug output

Usage: echo 42 | ./push --username=janesmith --password=foobar --database=my_sensortag --url=janesmith.cloudant.com
Usage: echo '{"foo":"bar"}' | ./push --username=janesmith --password=foobar --database=my_sensortag --url=janesmith.cloudant.com
```

## Requirements
- Node.js v0.12.x


## Logging use case

ECS fields used in logging use cases.

### <a name="logging"></a> Logging fields


| Field  | Description  | Type  | Multi Field  | Example  |
|---|---|---|---|---|
| <a name="id"></a>*id*  | *Unique id of the log entry.*  | keyword  |   | `8a4f500d`  |
| <a name="timestamp"></a>*timestamp*  | *Timestamp of the log line.*  | date  |   | `2016-05-23T08:05:34.853Z`  |
| [message](https://github.com/elastic/ecs#message)  | The log message.<br/>This can contain the full log line or based on the processing only the extracted message part. This is expected to be human readable.  | text  |   | `Hello World`  |
| <a name="hostname"></a>*hostname*  | *Hostname extracted from the log line.*  | keyword  |   | `www.example.com`  |
| <a name="ip"></a>*ip*  | *IP Address extracted from the log line. Can be IPv4 or IPv6.*  | ip  |   | `192.168.1.12`  |
| [log.level](https://github.com/elastic/ecs#log.level)  | Log level field. Is expected to be `WARN`, `ERR`, `INFO` etc.  | keyword  |   | `ERR`  |
| [log.line](https://github.com/elastic/ecs#log.line)  | Line number the log event was collected from.  | long  |   | `18`  |
| [log.offset](https://github.com/elastic/ecs#log.offset)  | Offset of the log event.  | long  |   | `12`  |
| [source.*](https://github.com/elastic/ecs#source.*)  | Describes from where the log entries come from.<br/>  |   |   |   |
| <a name="source.path"></a>*source.path*  | *File path of the file the data is harvested from.*  | keyword  |   | `/var/log/test.log`  |




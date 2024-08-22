# brontes db query

Query data from any libmdbx table and pretty print it in stdout

```bash
$ brontes db query --help
Usage: brontes db query [OPTIONS] --table <TABLE> --key <KEY>

Options:
  -t, --table <TABLE>
          Table to query

  -k, --key <KEY>
          Key for table query. Use Rust range syntax for ranges: --key 80 (single key) --key 80..100 (range)

      --brontes-db-path <BRONTES_DB_PATH>
          path to the brontes libmdbx db

  -h, --help
          Print help (see a summary with '-h')

  -V, --version
          Print version

Display:
  -v, --verbosity...
          Set the minimum log level.
          
          -v      Errors
          -vv     Warnings
          -vvv    Info
          -vvvv   Debug
          -vvvvv  Traces (warning: very verbose!)

      --quiet
          Silence all log output
```
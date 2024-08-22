# brontes db download-snapshot

Downloads a database snapshot. Without specified blocks, it fetches the full range. With start/end blocks, it downloads that range and merges it into the current database

```bash
$ brontes db download-snapshot --help
Usage: brontes db download-snapshot [OPTIONS]

Options:
      --endpoint <ENDPOINT>
          Snapshot endpoint
          
          [default: https://data.brontes.xyz/]

  -s, --start-block <START_BLOCK>
          Optional start block

      --brontes-db-path <BRONTES_DB_PATH>
          path to the brontes libmdbx db

  -e, --end-block <END_BLOCK>
          Optional end block

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
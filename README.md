# mongo-archive

Utility to archive a slice of a collection of documents in a Mongo database

## Usage

    usage: /usr/local/bin/mongo-archive [OPTIONS]

    OPTIONS:

          -b --expire-begin:           The beginning date of the expire period (default: 1 day before retention)
          -r --data-retention:         The number of days the data should stay online: data older thant this value will be archived [default:180]
          -s --skip-drop:              Skip documents removal from database, export documents only [default:false]
          -f --field-name:             The field to be used to check for age of data
          -c --collection:             MongoDB Collection
          -d --database:               MongoDB Database
          -h --host:                   MongoDB Host [default:localhost]
          -u --username:               MongoDB Username [default:root]
          -p --password:               MongoDB Password
          -q --quiet:                  Flag to set quiet mode on [default:false]
          -v --verbose:                Flag to set verbose mode on [default:false]
          -k --backup-dir:             Directory where to store backup files [default:/var/backups]
          -z --compress:               Gzip archived documents [default:false]
          -o --overwrite:              Overwrite archive files if existing [default:false]

          -? --help  :  usage

# Vendure Dev Server

This package is not published to npm. It is used in development of the Vendure server and plugins.

### Running

To run the server, run the `start` script. The database configuration can be specified by the `--db=<type>` flag:

```bash
yarn start --db=mysql
yarn start --db=postgres
yarn start --db=sqlite
```

The default if no db is specified is mysql.

### Populating data

Test data can be populated by running the `populate` script. This uses the same sample data as is used by the Vendure CLI when running `init`, albeit with the additional step of populating some sample customer & address data too.

Specify the database as above to populate that database:

```bash
yarn populate --db=sqlite
```
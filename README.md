# SQL Keep
Automate scheduled database dumps

Usage

- `./dump` This will generate a mysqldump in ./dumps folder, and the generated file name has the timestamp. Ex: `dump-20220116010525-mydbname.sql.gz`
- `./dump autodumps` This will generate a mysqldump in ./autodumps folder
- `./dump autodumps hourly` This will generate a mysqldump in ./autodumps folder, and the timestamp in the file name will be replace by 'hourly'. Ex: `hourly-mydbname.sql.gz`

For example, a cron job to take daily database backups would look like:

`0 0 * * * /path/to/dump autodumps daily`

Platforms Supported

- WordPress: Place this file alonside `wp-config.php` and it'll auto fetch database details from it


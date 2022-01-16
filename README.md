# dump
Automate scheduled database dumps

Usage

- `./dump` This will generate a mysqldump in ./dumps folder
- `./dump autodumps` This will generate a mysqldump in ./autodumps folder
- `./dump autodumps hourly` This will generate a mysqldump in ./autodumps folder, and the file name will be prefixed with 'hourly'

For example, a cron job to take daily database backups would look like:

`0 0 * * * /path/to/dump autodumps daily`

Platforms Supported

- WordPress: Place this file alonside `wp-config.php` and it'll auto fetch database details from it


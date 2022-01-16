# dump
Automate scheduled database dumps

Usage

- `./dump` This will generate a mysqldump in ./dumps folder
- `./dump autodumps` This will generate a mysqldump in ./autodumps folder
- `./dump autodumps hourly` This will generate a mysqldump in ./autodumps folder, and the file name will be prefixed with 'hourly'

Platforms Supported

- WordPress: Place this file alonside `wp-config.php` and it'll auto fetch database details from it

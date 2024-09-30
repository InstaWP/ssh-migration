# InstaWP SSH Migration

Note: This is alpha version, under heavy testing and development. You are welcome to try it out and provide feedback via [GitHub Issues](https://github.com/InstaWP/ssh-migration/issues).

Watch Demo - https://www.youtube.com/watch?v=0a-nOuThBvY


## Source Server

To use the InstaWP SSH Migration tool, you'll need to download the PHAR file. You can do this easily with the following one-liner command:

```bash
curl -sSL https://github.com/InstaWP/ssh-migration/releases/download/latest/source.phar -o source.phar && php source.phar
```

_Note: If the size of the source files are large, it is advisable to use screen or tmux to run the command in the background._

It will upload your entire website to the InstaWP cloud storage and output the backup_id.

## Destination Server

To download the destination server PHAR file, you can use the following command:

```bash
curl -sSL https://github.com/InstaWP/ssh-migration/releases/download/latest/dest.phar -o dest.phar && php dest.phar
```

## Manual Download and Execution

To use the SSH Migration tool:

1. Ensure PHP is installed on your system.
2. Download the PHAR file as shown above.
3. Make the PHAR file executable:
4. Run the PHAR file:

```bash
php source.phar
```

This will execute the SSH Migration tool and guide you through the migration process.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

# Changelog

## 1.0.1

- Add meta.json to store the version and other metadata.
- Refactor the code to use the meta.json file.
- Checksum the files and verify after download.
- Check if the website is empty before starting the migration.

## 1.0.0

- Initial release

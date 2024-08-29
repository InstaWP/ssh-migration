# InstaWP SSH Migration

## Source Server

To use the InstaWP SSH Migration tool, you'll need to download the PHAR file. You can do this easily with the following one-liner command:

```bash
curl -sSL https://github.com/InstaWP/ssh-migration/releases/latest/download/source.phar -o source.phar 
```

It will upload your entire website to the InstaWP cloud storage and output the backup_id.

## Destination Server

To download the destination server PHAR file, you can use the following command:

```bash
curl -sSL https://github.com/InstaWP/ssh-migration/releases/latest/download/dest.phar -o dest.phar backup_id
```

## Manual Download and Execution

To use the SSH Migration tool:

1. Ensure PHP is installed on your system.
2. Download the PHAR file as shown above.
3. Make the PHAR file executable:

```bash
chmod +x source.phar
```

4. Run the PHAR file:

```bash
./source.phar
```

This will execute the SSH Migration tool and guide you through the migration process.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

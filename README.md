# Swiss Parks PHP SDK (legacy)

Frozen archive of **MySQL-based** Swiss Parks PHP API / SDK packages (**v14–v21.1**).

This repository is **not** under active development. Use it only to download historical release ZIPs.

## Current SDK

From **v22** onward the SDK uses SQLite and lives in a separate repository:

- [indual-web/swiss-parks-php-sdk](https://github.com/indual-web/swiss-parks-php-sdk)
- Migration **v21 → v22**: [docs/guides/migrations/21-to-22.md](https://github.com/indual-web/swiss-parks-php-sdk/blob/main/docs/guides/migrations/21-to-22.md)

## Available packages

ZIP files are in [`releases/`](./releases/):

| Version | File | Notes |
| --- | --- | --- |
| 14 | [swiss-parks-php-sdk-14.zip](./releases/swiss-parks-php-sdk-14.zip) | MySQL, folder `parks_api/` |
| 15 | [swiss-parks-php-sdk-15.zip](./releases/swiss-parks-php-sdk-15.zip) | MySQL, folder `parks_api/` |
| 16 | [swiss-parks-php-sdk-16.zip](./releases/swiss-parks-php-sdk-16.zip) | MySQL, folder `parks_api/` |
| 17 | [swiss-parks-php-sdk-17.zip](./releases/swiss-parks-php-sdk-17.zip) | MySQL, folder `parks_api/` |
| 18 | [swiss-parks-php-sdk-18.zip](./releases/swiss-parks-php-sdk-18.zip) | MySQL, folder `parks_api/` |
| 19 | [swiss-parks-php-sdk-19.zip](./releases/swiss-parks-php-sdk-19.zip) | MySQL, folder `parks_api/` |
| 20 | [swiss-parks-php-sdk-20.zip](./releases/swiss-parks-php-sdk-20.zip) | MySQL, folder `parks_api/` |
| 21 | [swiss-parks-php-sdk-21.zip](./releases/swiss-parks-php-sdk-21.zip) | MySQL, folder `parks_api/` |
| 21.1 | [swiss-parks-php-sdk-21.1.zip](./releases/swiss-parks-php-sdk-21.1.zip) | MySQL, folder `parks_api/` |

Each package includes `parks_api/classes/ParksMigration.php` with incremental schema steps up to that version. Within the MySQL line, upgrade by replacing API files (keep `config.php` / `custom/`) and running `scripts/migrate.php` as described in the package `README.txt`.

## Support status

- **Unsupported** for new integrations
- No new builds, fixes, or migration guides for steps before v21
- Prefer upgrading to **v21.1**, then to **v22** using the current SDK docs

## License

Same terms as the current SDK: see [LICENSE](./LICENSE). Use is limited to member parks of the Network of Swiss Parks.

## Contact

[parks.swiss](https://www.parks.swiss) · [info@parks.swiss](mailto:info@parks.swiss)

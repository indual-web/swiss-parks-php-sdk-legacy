# Swiss Parks PHP SDK (legacy)

Frozen archive of **MySQL-based** Swiss Parks PHP API / SDK packages (**v14–v21.1**).

This repository is **not** under active development. Use it only to download historical release ZIPs.

## Current SDK

From **v22** onward the SDK uses SQLite and lives in a separate repository:

- [indual-web/swiss-parks-php-sdk](https://github.com/indual-web/swiss-parks-php-sdk)
- Migration **v21 → v22**: [docs/guides/migrations/21-to-22.md](https://github.com/indual-web/swiss-parks-php-sdk/blob/main/docs/guides/migrations/21-to-22.md)

## Available packages

ZIP files are in [`releases/`](./releases/). Frozen per-version upgrade notes (formerly in the Offer Database export settings) are in [`docs/migrations/`](./docs/migrations/index.md).

| Version | File | Migration |
| --- | --- | --- |
| 14 | [swiss-parks-php-sdk-14.zip](./releases/swiss-parks-php-sdk-14.zip) | [docs/migrations/14.md](./docs/migrations/14.md) |
| 15 | [swiss-parks-php-sdk-15.zip](./releases/swiss-parks-php-sdk-15.zip) | [docs/migrations/15.md](./docs/migrations/15.md) |
| 16 | [swiss-parks-php-sdk-16.zip](./releases/swiss-parks-php-sdk-16.zip) | [docs/migrations/16.md](./docs/migrations/16.md) |
| 17 | [swiss-parks-php-sdk-17.zip](./releases/swiss-parks-php-sdk-17.zip) | [docs/migrations/17.md](./docs/migrations/17.md) |
| 18 | [swiss-parks-php-sdk-18.zip](./releases/swiss-parks-php-sdk-18.zip) | [docs/migrations/18.md](./docs/migrations/18.md) |
| 19 | [swiss-parks-php-sdk-19.zip](./releases/swiss-parks-php-sdk-19.zip) | [docs/migrations/19.md](./docs/migrations/19.md) |
| 20 | [swiss-parks-php-sdk-20.zip](./releases/swiss-parks-php-sdk-20.zip) | [docs/migrations/20.md](./docs/migrations/20.md) |
| 21 | [swiss-parks-php-sdk-21.zip](./releases/swiss-parks-php-sdk-21.zip) | [docs/migrations/21.md](./docs/migrations/21.md) |
| 21.1 | [swiss-parks-php-sdk-21.1.zip](./releases/swiss-parks-php-sdk-21.1.zip) | [docs/migrations/21.1.md](./docs/migrations/21.1.md) |

Each package includes `parks_api/classes/ParksMigration.php` with incremental schema steps up to that version. Keep `config.php` / `custom/` when replacing API files, then run `scripts/migrate.php` as in the version guide and package `README`.

## Support status

- **Unsupported** for new integrations
- No new builds or fixes; migration notes above are frozen archives
- Prefer upgrading to **v21.1**, then to **v22** using the current SDK docs

## License

Same terms as the current SDK: see [LICENSE](./LICENSE). Use is limited to member parks of the Network of Swiss Parks.

## Contact

[parks.swiss](https://www.parks.swiss) · [info@parks.swiss](mailto:info@parks.swiss)

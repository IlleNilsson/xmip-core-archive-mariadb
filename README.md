# xmip-core-archive-mariadb

MariaDB archive target: one item is one row of an archive table. A technology of [xmip-core-archive](https://github.com/IlleNilsson/xmip-core-archive).

The store is the capability's `archive::sql::SqlArchive`; this crate is its
`archive::sql::Database`, `MariaDb` — the SQL the server speaks (`MariaDB`'s, `sql::MARIADB`,
from `xmip-core-library-sql`) and the connection through
[xmip-core-library-mariadb](https://github.com/IlleNilsson/xmip-core-library-mariadb),
the protocol the MariaDB transport speaks too.
An archive here is `SqlArchive::<MariaDb>::new(server, database, user)`.

## Toolchain

`rust-toolchain.toml` pins the toolchain for the whole estate. Do not change it
here.

## Verification

The included workflow is manual-only and calls the versioned shared workflow at
`IlleNilsson/.github@v1`.

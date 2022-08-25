# A Demo with Laravel + CrateIo + Jetstream

# Notes

## CrateIo

Big things that are not supported are:

- joins
- subselects
- auto increments - you'll have to manage those by yourself
- whereBetween(s)
- unique indexes
- foreign keys (and relations)
- dropping, renaming columns (adding fields works)
- naming columns like _ id, _ version, _ score - these are restricted, crate uses it internally

Crate specific stuff that were added are:

- object type
- array type
- index off, index plain
- fulltext indexes over single or multiple fields w/o analyzers
- table partitioning
- generated columns

# Changelog - amazonka-s3-streaming

## 0.2.0.0
 * Fixed a potential bug with very large uploads where the chunksize might be too small
   for the limit of 10,000 chunks per upload (#6).
 * Change API to allow the user to specify a chunk size for streaming if the user knows
   more about the data than we do.
 * Allow the user to specify how many concurrent threads to use for `concurrentUpload` as
   as well as chunk size (#4).
 * Better specify cabal dependency ranges.
# Selectel supload

```
Usage:
    supload.sh [-a AUTH_URL] -u <USER> -k <KEY> [-r] [[-e PATTERN]...] [options] <dest_dir> <src_path>

Options:
    -a AUTH_URL    authentication url (default: https://auth.selcdn.ru/)
    -u USER        user name
    -k KEY         user password
    -r             recursive upload
    -M             force upload without check by md5 sum
    -e PATTERN     exclude files by pattern (shell pattern syntax, ex. .git/*)
    -d NUM<m:h:d>  auto delete file in storage after NUM minutes or hours or days (ex. 7d)
    -s NUM<K:M:G>  specify the maximum transfer rate you want use to upload (ex. 1M)
    -m FILTER      add MTIME filter. Usefull to upload only new files in large directory (find -mtime syntax, ex. -1)
    -z FORMAT      Treat file as archive of a given type and extract it after upload. Supported formats: tar, tar.gz, tar.bz2
    -c             enable detect mime type for file and set content-type for uploading file (usually the storage can do it self)
    -q             quiet mode (error output only)

Params:
     <dest_dir>    destination directory or container in storage (ex. container/dir1/), not a file name
     <src_path>    source file or directory
```

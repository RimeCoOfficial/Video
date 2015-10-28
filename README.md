# Assets-videos

## `.gitattributes`
Example: https://github.com/lsst/git-lfs-more-testing/blob/master/.gitattributes
```sh
*.mov filter=lfs diff=lfs merge=lfs -text
```

Find largest file http://superuser.com/questions/9847/linux-utility-for-finding-the-largest-files-directories
```
$ find . -type f -print0 | xargs -0 du | sort -rn | head -10 | cut -f2 | xargs -I{} du -sh {}

  346M   ./Downloads/The Walking Dead S02E02 ... (dutch subs nl).avi
  159M   ./.local/share/Trash/files/funky chicken.mpg
  117M   ./Calibre Library/Robert Martin/cc.mobi
  114M   ./Dropbox/snapshots/monthly.tgz
  114M   ./Dropbox/snapshots/daily.tgz
  114M   ./Dropbox/snapshots/weekly.tgz
  76M    ./tmp/projects/onthisday/onthisday.tar.gz
  76M    ./snapshots/projects/weekly.3/onthisday/onthisday.tar.gz
  76M    ./snapshots/projects/weekly.2/onthisday/onthisday.tar.gz
  76M    ./snapshots/projects/weekly.1/onthisday/onthisday.tar.gz
```

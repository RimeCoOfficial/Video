# Videos

<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/StillImage" property="dct:title" rel="dct:type">Videos</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://rime.co" property="cc:attributionName" rel="cc:attributionURL">Rime</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/RimeOfiicial" rel="dct:source">https://github.com/RimeOfiicial</a>.

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

Find extentions count http://stackoverflow.com/questions/1842254/how-can-i-find-all-of-the-distinct-file-extensions-in-a-folder-hierarchy
```
$ find . -type f -name "*.*" | grep -o -E "\.[^\.]+$" | sort | uniq -c | sort -rn

 353 .JPG
  53 .png
  45 .mov
  33 .DS_Store
  15 .prproj
     ...
   2 .MXF
   1 .xmp
   1 .psd
   1 .mp4
   1 .md
   1 .m4a
   1 .gitignore
   1 .gitattributes
```


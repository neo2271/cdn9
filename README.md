 ### [The index.html file lists all files/directories:](https://stackoverflow.com/a/46383157)

    tree -H '.' --noreport --charset utf-8 -P "*" > showme.html

    tree -H '.' --noreport --charset utf-8 -P "*.*" > showme.html

    md5deep * -z -l | awk '{print $2,$3,$1}'

    md5deep *.zip -z -l | awk '{print $2,$3,$1}'

    md5deep *.* -z -l | awk '{print $2,$3,$1}'

    md5deep * -z -l | awk '{print $2 " | " $3 " | " $1}'

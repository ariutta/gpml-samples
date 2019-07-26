# gpml-samples

Random samples of GPML files

gpmlfile=$(ls -1 2017 | head -1); wpid=$(echo $gpmlfile | awk -F_ '{print $(NF-1)}'); mv 2017/$gpmlfile ./gpml/$wpid.gpml; gpmlfile2019=$(ls -1 2019 | head -1); wpid2019=$(echo $gpmlfile2019 | awk -F_ '{print $(NF-1)}'); mv 2019/$gpmlfile2019 ./gpml/$wpid2019.gpml; git add gpml/; git commit -am "Add/update $wpid and $wpid2019"; git push

 #!/bin/bash
url=$1
if [ ! -d "$url" ];then
mkdir $url


fi


if [ ! -d "$url/recon" ];then
mkdir $url/recon


fi
echo "[+] Hunteing Subdomains with Asstfinder.. "                                                                                                                        
  
assetfinder $url >> $url/recon/assets.txt


cat $url/recon/assets.txt | grep $1 >> $url/recon/assets.txt


rm $url/recon/assets.txt

# bash
one-liners
while read password; do unzip -P "$password" Documents.zip && echo "Success with password: $password" && break || echo "Failed: $password"; done < numbers83.txt

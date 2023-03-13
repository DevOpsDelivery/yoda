# Linux basics LAB2

## Exercises

Do the next exercises per order.


1. Display the size and type of file of /bin/cat, /etc/passwd and /usr/bin/passwd
ls -lh /bin/cat /etc/passwd /usr/bin/passwd
2. Download logo-d2si.png and d2si-mag-nouveaux-mc3a9tiers_2015.pdf using wget
    - https://www.w3.org/WAI/ER/tests/xhtml/testfiles/resources/pdf/dummy.pdf
    - https://d33wubrfki0l68.cloudfront.net/b5759d3228a9bc5fcf2a87cb7175eafc1d417c4b/4de06/events/2023-melbourne/logo.png

3. Display the type of file of logo-.png  and dummy.pdf
file  logo.png dummytest.pdf
4. Rename logo-d2si.png to logo-d2si.pdf
mv dummy.pdf dummytest.pdf
5. Display the type of file of logo-d2si.pdf and d2si-mag-nouveaux-mc3a9tiers_2015.pdf
file  logo.pdf dummytest.pdf
logo.pdf:      PNG image data, 2038 x 1568, 8-bit/color RGBA, non-interlaced
dummytest.pdf: PDF document, version 1.4

6. Create a directory ~/touched and enter it
mkdir ~/touched && cd ~/touched

7. Create the files today.txt and yesterday.txt in touched
touch today.txt yesterday.txt

8. Change the date on yesterday.txt to match yesterday's date
touch -d "yesterday" yesterday.txt

9. Copy yesterday.txt to copy.yesterday.txt
cp yesterday.txt copy.yesterday.txt

10. Create a directory called ~/testbackup and copy all files from ~/touched in it
mkdir ~/testbackup && cp -r ~/touched/* ~/testbackup/

11. Use one command to remove the directory ~/testbackup and all files in it
rm -r ~/testbackup/
12. Create a directory ~/etcbackup and copy all *.conf files from /etc in it. Did you include all subdirectories of /etc ?
mkdir ~/etcbackup && sudo find /etc -type f -name "*.conf" -exec cp --parents {} ~/etcbackup \;

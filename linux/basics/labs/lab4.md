# Linux basics LAB4

## Exercises

Do the next exercises per order.


1. List all files in /etc ending with “.conf”
ls -l /etc/*.conf
2. List all commands in /bin starting with “mk”
ls -l /bin/mk*
3. List all commands in /bin containing digits
ls /bin/*[0-9]*
4. List all directories in /etc containing digits
ls -d /etc/*[0-9]*
5. List all files in /boot with name containing a dot (“.”) or a dash (“-”)
ls -l /boot/*[.-]*
6. List all files in /etc using echo(1)
echo /etc/*
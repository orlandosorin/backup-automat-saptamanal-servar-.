
gedit /usr/local/bin/backup.sh

editeaza executabilul cu ce ai tu in servar

Pe urma deschide crontab -e in root si editeaza:

0 3 * * 1 /usr/local/bin/backup.sh >> /var/log/backup_cron.log 2>&1

03 = ora la care se face backup automat; 1 - luni;

0 sau 7 = Duminică1 = Luni (ceea ce ai tu setat)2 = Marți3 = Miercuri4 = Joi5 = Vineri6 = Sâmbătă

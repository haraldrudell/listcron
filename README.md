# listcron

List cron jobs on Debian/Ubuntu by Harald Rudell

```
$ sudo listcron
===  c89:listcron:9287 2001-01-06 02:01:28-08:00
[crontab] SHELL=/bin/sh
[crontab] PATH=/usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin
[crontab] 17 *  * * *   root    cd / && run-parts --report /etc/cron.hourly
[cron.d:anacron] SHELL=/bin/sh
[cron.d:anacron] PATH=/usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin
[cron.d:anacron] 30 7    * * *   root   test -x /etc/init.d/anacron && /usr/sbin/invoke-rc.d anacron start >/dev/null
[cron.d:logwatch] 1 0 * * * root /usr/sbin/logwatch --output mail
[cron.daily] 0anacron
[cron.monthly] 0anacron
===  listcron completed successfully in 0.2 s
$ listcron --help


===  c89:listcron:9700 1980-12-23 07:41:32-08:00
Usage: listcron [options] file
List all cron jobs for all users
  --quiet suppress display of non-essential output
```

Debian provides /etc/cron.d and more which this utility lists as opposed to crontab -l

# Notes

© [Harald Rudell](http://www.haraldrudell.com) wrote this in 2015

No warranty expressed or implied. Use at your own risk.



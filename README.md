Squid-BlackList
===============

Black list for Squid proxy.

Tips
===============
  * Example of crontab rule for automatic update every first day of the month:
<code>
0       6       1       *       *       root    /usr/bin/fetch -q -o /usr/local/etc/squid/denied_ext.conf https://raw.github.com/oleksiig/Squid-BlackList/master/denied_ext.conf && /usr/local/etc/rc.d/squid reload
</code>
<i>NOTE: This rule related to the FreeBSD default patches so double check before use on other platforms</i>

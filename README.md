### fastmail-ldap

Query
[FastMail's](https://www.fastmail.com/)
LDAP server from
[Mutt](http://www.mutt.org/)
when completing aliases.

Edit `fastmail-ldap.pl` and set `$username` and `$password`.

In your `~/.muttrc` file, call this script as `query_command`:

	set query_command="~/bin/fastmail-ldap.pl '%s'"

Tip: to complete addresses with the Tab key instead of Control+T, set:

	bind editor <tab> complete-query

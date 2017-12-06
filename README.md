# weesms

2015-04-12: v0.1 - Initial/draft/beta version

Installation
------------

$ sudo aptitude install gammu gammu-smsd python-gammu
$ sudo usermod -a -G dialout $USER

$ cp weesms.py ~/.weechat/python/[autoload]

Stop gammu-smsd if it is started:
/etc/init.d/gammu-smsd stop


Plugin management
-----------------

Load plugin:
/python load python/weesms.py or put the script in python/autoload

Reload plugin:
/python reload weesms

Unload plugin:
/python unload weesms


Phonebook
---------

Default CSV phonebook location: WEECHAT_DIR/python/weesms.csv

Phonebook format is:
bob,+33123456789
alice,+33987654321


Refs:
  - http://wammu.eu/docs/pdf/gammu.pdf
  - https://weechat.org/files/doc/stable/weechat_scripting.en.html
  - https://weechat.org/files/doc/stable/weechat_plugin_api.en.html


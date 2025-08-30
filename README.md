jk_checkpproc
==========

Introduction
------------

This python module provides a python script that checks if a specified program is a parent of the current process.

Information about this module can be found here:

* [github.org](https://github.com/jkpubsrc/python-tool-jk-checkpproc)
* [pypi.python.org](https://pypi.python.org/pypi/jk-checkpproc)

Why this tool?
----------------

This tool can be used as part of `.bashrc` to detect if the current session is a ssh remote login session or not.
If so you can set the prompt accordingly.

Example:

```bash
if jkcheckpproc.py -c sshd; then
	# set your custom prompt here
	PS1=....
else
	# use the standard prompt
	PS1=${debian_chroot:+($debian_chroot)}\u@\h:\w\$
fi
```

Contact Information
-------------------

* Jürgen Knauth: pubsrc@binary-overflow.de

License
-------

This software is provided under the following license:

* Apache Software License 2.0




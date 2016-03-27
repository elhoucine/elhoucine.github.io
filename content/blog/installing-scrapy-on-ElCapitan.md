+++

date = "2016-03-27T19:19:31+01:00"

draft = false

title = "Installing scrapy on El Capitan"

+++

If you are trying to install Scrapy *globally* via pip on El Capitan, you may go through some trouble related to [six](https://pypi.python.org/pypi/six).

```
OSError: [Errno 1] Operation not permitted: '/var/folders/2r/m12cht2j3332gy6tlqd66xmw0000gn/T/pip-tAYZND-uninstall/System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python/six-1.4.1-py2.7.egg-info'
```

You can read more about this [issue](https://github.com/pypa/pip/issues/3165).

To fix this you can use virtualenv or simply install Python using brew:

``
brew install python
``

And then:

``
sudo pip install scrapy
``

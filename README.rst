Note
=========
Dieser Fork ist aus (https://pypi.python.org/pypi/pyrocksdb/0.4) abgeleitet. Im Original mit 'pip install python-rocksdb' habe ich eine 'wheel'-Fehlermeldung erhalten.
Deshalb habe ich das Original neu gepackt und auf https://pypi.org/project/py3-rocksdb veröffentlicht



    $ pip3 install virtualenv

    $ virtualenv venv

    $ source venv/bin/activate

    $ pip3 install py3-rocksdb

    $ python3

    >>> import rocksdb
    >>> db = rocksdb.DB("test.db", rocksdb.Options(create_if_missing=True))
    >>> db.put(b'a', b'data')
    >>> print db.get(b'a')
    b'data'

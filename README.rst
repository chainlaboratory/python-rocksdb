Note
=========
The original pyrocksdb (https://pypi.python.org/pypi/pyrocksdb/0.4) has not been updated for long time. I update pyrocksdb to support the latest rocksdb. Please open issues in github if you have any problem.



    $ pip install py3-rocksdb

    >>> import rocksdb
    >>> db = rocksdb.DB("test.db", rocksdb.Options(create_if_missing=True))
    >>> db.put(b'a', b'data')
    >>> print db.get(b'a')
    b'data'

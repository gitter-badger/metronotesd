[![Build Status](https://travis-ci.org/Metronotes/metronotesd.svg?branch=develop)](https://travis-ci.org/Metronotes/metronotesd)
[![Build Status](https://circleci.com/gh/Metronotes/metronotesd.svg?&style=shield)](https://circleci.com/gh/Metronotes/metronotesd)
[![Coverage Status](https://coveralls.io/repos/Metronotes/metronotesd/badge.png?branch=develop)](https://coveralls.io/r/Metronotes/metronotesd?branch=develop)
[![Latest Version](https://pypip.in/version/metronotes-lib/badge.svg)](https://pypi.python.org/pypi/metronotes-lib/)
[![License](https://pypip.in/license/metronotes-lib/badge.svg)](https://pypi.python.org/pypi/metronotes-lib/)
[![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/Metronotes/General)


# Description
`metronotes-lib` is the reference implementation of the [Metronotes Protocol](https://metronotes.io).


# Requirements
* [Patched Bitcoin Core](https://github.com/btcdrak/bitcoin/releases) with the following options set:

	```
	rpcuser=bitcoinrpc
	rpcpassword=<password>
	server=1
	txindex=1
	addrindex=1
	rpcthreads=1000
	rpctimeout=300
	```


# Installation

```
$ git clone https://github.com/Metronotes/metronotesd.git
$ cd metronotesd
$ python3 setup.py install
```


# Usage

```
$ python3
>>> from metronoteslib import server
>>> db = server.initialise(<options>)
>>> server.start_all(db)
```


# Further Reading

* [Official Project Documentation](http://metronotes.io/docs/)

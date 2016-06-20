# Quickstart

This page has instructions to set up a single stand-alone BigchainDB node for learning or experimenting. If you want to set up a BigchainDB node for production, development, benchmarking, or something else, see the [BigchainDB Nodes](nodes/index.html) section.

We will assume you're using Ubuntu 14.04 or similar. If you're not using Linux, then you might try [running BigchainDB with Docker](nodes/run-with-docker.html).

A. [Install RethinkDB Server](https://rethinkdb.com/docs/install/ubuntu/)

B. Open a Terminal and run RethinkDB Server with the command:
```text
rethinkdb
```

C. Ubuntu 14.04 already has Python 3.4, so you don't need to install it, but you do need to install a couple other things:
```text
sudo apt-get update
sudo apt-get install g++ python3-dev
```

D. Get the latest version of pip, wheel and setuptools:
```text
sudo apt-get install python3-setuptools
sudo easy_install3 pip
pip3 install --upgrade pip wheel setuptools
```

E. Install the `bigchaindb` Python package from PyPI:
```text
sudo pip install bigchaindb
```

F. Configure and run BigchainDB:
```text
bigchaindb -y configure
bigchaindb start
```

That's it!

For now, you can get a good sense of how to work with BigchainDB by going through [the examples in the section on the Python Server API](nodes/python-server-api-examples.html).
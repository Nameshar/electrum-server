Electrum-server for the Electrum client
=========================================

  * Author: thomasv@bitcointalk
  * Language: Python
  * Edited for PTS by: barwizi PiNEJGUv4AZVZkLuF6hV4xwbYTRp5etWWJ

Features
--------

  * The server uses a Protosharesd and a leveldb backend.
  * The server code is open source. Anyone can run a server, removing single
    points of failure concerns.
  * The server knows which set of Protoshares addresses belong to the same wallet,
    which might raise concerns about anonymity. However, it should be possible
    to write clients capable of using several servers.

Installation
------------

  1. To install and run a pruning server (easiest setup) see README.leveldb
  2. Install [jsonrpclib](https://github.com/joshmarshall/jsonrpclib).
  3. Launch the server: `nohup python -u server.py > /var/log/electrum.log &`
     or use the included `start` script.

See the included `HOWTO.md` for greater detail on the installation process.

License
-------

Electrum-server is made available under the terms of the [GNU Affero General
Public License](http://www.gnu.org/licenses/agpl.html), version 3. See the 
included `LICENSE` for more details.

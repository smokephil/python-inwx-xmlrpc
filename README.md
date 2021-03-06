# python-inwx-xmlrpc: A Python class to simplify and leverage the communication with the XML-RPC API of InterNetworX via Python.

## Project Information

This software (python-inwx-xmlrpc) provides an easy way to use the XMLRPC API
offered by InterNetworX to its customers.
The software consists of a class to leverage the use of the API
and example code to show how to use it.

If you have an idea for the software or want to report a bug, let me know via
email!

## Required Python modules

The software is tested and known to work well on **Python 2.7.1** on Mac OS X 10.6.7.
It should, however, work on any operating system that supports python.
I also tested it on **Python 3.2** after converting the files using `2to3-3.2 -w -n *.py`. All examples were tested afterwards and found to be functional.

Python modules used in this software include the standard modules xmlrpclib, ConfigParser and sys.

## Installation and Usage

1. Get the source code of the project (via .tar.gz or .zip download or via git).
2. Duplicate the configuration file `python-inwx-xmlrpc.cfg.example` to `python-inwx-xmlrpc.cfg` and enter your credentials in the section [live].
3. Try out the examples to find out if it's working.
  1. Test the example script `example.list-domains.py`. If this prints a list of all your domains, the connection and use of the API is working.
  2. Test the other example scripts (you may need to adjust more sections in the configuration file).
4. If you want to use the class in your own projects and with more *remote procedure calls*,
   you should have look at the API documentation PDF: xmlrpc.pdf contained in
   [the official API .zip file](https://www.inwx.de/de/download/file/api-current.zip) (only accessible to customers).
   For example, if you want to use the command listInvoices from the accounting object, then do it like this:
   `inwx_conn.accounting.listInvoices()`  
   For a short overview about what's possible with the API, have a look at the wiki site [Available Objects](https://github.com/pklaus/python-inwx-xmlrpc/wiki/Available-Objects).

Please refer to my blog post, where I presented the class:
<http://blog.philippklaus.de/2011/05/access-the-internetworx-xml-rpc-api-via-python/>
for more information on this class and how you can use it.

## License

> python-inwx-xmlrpc is free software: you can redistribute it and/or modify
> it under the terms of the GNU General Public License as published by
> the Free Software Foundation, either version 3 of the License, or
> (at your option) any later version.
> 
> python-inwx-xmlrpc is distributed in the hope that it will be useful,
> but WITHOUT ANY WARRANTY; without even the implied warranty of
> MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
> GNU General Public License for more details.
> 
> You should have received a copy of the GNU General Public License
> along with python-inwx-xmlrpc.  If not, see <http://www.gnu.org/licenses/>.

## Author

* Philipp Klaus
  * Web site: <http://www.philippklaus.de>
  * Email: philipp.klaus →AT→ gmail.com
* InterNetworX
  * Web site: <http://inwx.de>
  * Email: info →AT→ inwx.de

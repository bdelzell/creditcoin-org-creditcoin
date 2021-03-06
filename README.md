Creditcoin Core integration/staging tree
=====================================

[![Build Status](https://creditcoin.io/creditcoin-project/creditcoin.svg?branch=master)](https://creditcoin.io/creditcoin-project/creditcoin)

https://creditcoin.net

What is The Credit?
----------------

The Credit is a digital currency that enables instant payments to
anyone, anywhere in the world. The Credit uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. Credit Core is the name of the open source
software which enables the use of this currency. It is based upon Litecoin and 
has its roots in the bitcoin original blockchain. The Credit has 8 times the amount
of available currency in its blockchain, and with a 10% premine in escrow to give a
solid base to the currency and guard against future inflation. Any gains on escrow value will be 
transfered to non-profit orginizations that will pursue green technology and upright social values
from a street level.

For more information, as well as an immediately useable, binary version of
the Credit Core software, see [https://creditcoin.net](https://creditcoin.net
).

License
-------

The Credit Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/litecoin-project/litecoin/tags) are created
regularly to indicate new official, stable release versions of Litecoin Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

The developer [mailing list](https://groups.google.com/forum/#!forum/creditcoin-dev)
should be used to discuss complicated or controversial changes before working
on a patch set.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](/doc/unit-tests.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`

There are also [regression and integration tests](/qa) of the RPC interface, written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/qa) are installed) with: `qa/pull-tester/rpc-tests.py`


### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

We only accept translation fixes that are submitted through [Bitcoin Core's Transifex page](https://www.transifex.com/projects/p/bitcoin/).
Translations are converted to the Credit core periodically.

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.

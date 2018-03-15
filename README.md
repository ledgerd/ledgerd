
# ledgerd - LedgerD server
`ledgerd` is the reference server implementation of the LedgerD
protocol. To learn more about how to build and run a `ledgerd`
server, visit https://ledgerd.org/build/ledgerd-setup/

## Build
- **install boost**  
  $ sudo apt install libboost-all-dev
- **install protobuf**  
  $ sudo apt-get install autoconf automake libtool curl make g++ unzip  
  $ wget https://github.com/google/protobuf/releases/download/v3.5.1/protobuf-all-3.5.1.tar.gz  
  $ tar -xzvf protobuf-all-3.5.1.tar.gz  
  $ cd protobuf-3.5.1  
  $ ./configure --prefix=/usr  
  $ make  
  $ make check  
  $ sudo make install  
  $ sudo ldconfig  
- **install other deps**  
  $ sudo apt install openssl  
  $ sudo apt install libssl-dev  
  $ sudo apt install pkg-config  
  $ sudo apt install scons  
- **compile**  
  $ sudo apt install git  
  $ git clone https://gitlab.com/ledgerd/ledgerd.git  
  $ cd ledgerd  
  $ sudo scons  

[![travis-ci.org: Build Status](https://travis-ci.org/ripple/rippled.png?branch=develop)](https://travis-ci.org/ripple/rippled)
[![codecov.io: Code Coverage](https://codecov.io/gh/ripple/rippled/branch/develop/graph/badge.svg)](https://codecov.io/gh/ripple/rippled)

### License
`ledgerd` is open source and permissively licensed under the
ISC license. See the LICENSE file for more details.

#### Repository Contents

| Folder  | Contents |
|---------|----------|
| ./bin   | Scripts and data files for Ripple integrators. |
| ./build | Intermediate and final build outputs.          |
| ./Builds| Platform or IDE-specific project files.        |
| ./doc   | Documentation and example configuration files. |
| ./src   | Source code.                                   |

Some of the directories under `src` are external repositories inlined via
git-subtree. See the corresponding README for more details.


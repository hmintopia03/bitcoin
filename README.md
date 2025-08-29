<<<<<<< HEAD
Bitcoin Core integration/staging tree
=====================================

https://bitcoincore.org

For an immediately usable, binary version of the Bitcoin Core software, see
https://bitcoincore.org/en/download/.

What is Bitcoin Core?
---------------------

Bitcoin Core connects to the Bitcoin peer-to-peer network to download and fully
validate blocks and transactions. It also includes a wallet and graphical user
interface, which can be optionally built.

Further information about Bitcoin Core is available in the [doc folder](/doc).

License
-------

Bitcoin Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built (see `doc/build-*.md` for instructions) and tested, but it is not guaranteed to be
completely stable. [Tags](https://github.com/bitcoin/bitcoin/tags) are created
regularly from release branches to indicate new official, stable release versions of Bitcoin Core.

The https://github.com/bitcoin-core/gui repository is used exclusively for the
development of the GUI. Its master branch is identical in all monotree
repositories. Release branches and tags do not exist, so please do not fork
that repository unless it is for development reasons.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md)
and useful hints for developers can be found in [doc/developer-notes.md](doc/developer-notes.md).

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).

There are also [regression and integration tests](/test), written
in Python.
These tests can be run (if the [test dependencies](/test) are installed) with: `test/functional/test_runner.py`

The CI (Continuous Integration) systems make sure that every pull request is built for Windows, Linux, and macOS,
and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

Changes to translations as well as new translations can be submitted to
[Bitcoin Core's Transifex page](https://www.transifex.com/bitcoin/bitcoin/).

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.
=======
# bitcoin
# Bitcoin Core (Personal Modified Version)

## English
This repository is a **personal modified version of Bitcoin Core**,  
originally based on the old 2015 codebase.  
Some corrections and small adjustments have been made in order to:  
- Keep a personal record of changes  
- Use as a study and practice resource for blockchain technology  
- Experiment with building and running a node in a modern environment  

**⚠️ Note:**  
This is **not** the official Bitcoin Core repository.  
The official project lives at: [github.com/bitcoin/bitcoin](https://github.com/bitcoin/bitcoin)

---

## 한국어
이 저장소는 **비트코인 코어의 개인 수정 버전**입니다.  
2015년의 오래된 코드를 기반으로 하였으며, 다음과 같은 목적을 위해 일부 수정 및 보완을 했습니다:  
- 개인적인 수정 내역 기록  
- 블록체인 **공부/연습용 자료**로 활용  
- 현대 환경에서 노드 실행/빌드를 실험  

**⚠️ 주의:**  
이 저장소는 **공식 비트코인 코어 저장소가 아닙니다.**  
공식 프로젝트는 [github.com/bitcoin/bitcoin](https://github.com/bitcoin/bitcoin) 에서 확인하세요.

---

## How to Build & Run (빌드 및 실행 방법)

### Build
```bash
./autogen.sh
./configure
make
>>>>>>> 700f4ce2f662e521eeb8425750c7549bd04a6ec0

d8054ad1dea03a34bffcb4741cbfef9b8658b39c The web-platform-tests Project
==============================

[![Taskcluster CI Status](https://community-tc.services.mozilla.com/api/github/v1/repository/web-platform-tests/wpt/master/badge.svg)](https://community-tc.services.mozilla.com/api/github/v1/repository/web-platform-tests/wpt/master/latest) [![documentation](https://github.com/web-platform-tests/wpt/workflows/documentation/badge.svg)](https://github.com/web-platform-tests/wpt/actions?query=workflow%3Adocumentation+branch%3Amaster) [![manifest](https://github.com/web-platform-tests/wpt/workflows/manifest/badge.svg)](https://github.com/web-platform-tests/wpt/actions?query=workflow%3Amanifest+branch%3Amaster) [![Python 3](https://pyup.io/repos/github/web-platform-tests/wpt/python-3-shield.svg)](https://pyup.io/repos/github/web-platform-tests/wpt/)

The web-platform-tests Project is a cross-browser test suite for the
Web-platform stack. Writing tests in a way that allows them to be run in all
browsers gives browser projects confidence that they are shipping software that
is compatible with other implementations, and that later implementations will
be compatible with their implementations. This in turn gives Web
authors/developers confidence that they can actually rely on the Web platform
to deliver on the promise of working across browsers and devices without
needing extra layers of abstraction to paper over the gaps left by
specification editors and implementors.

The most important sources of information and activity are:

- [github.com/web-platform-tests/wpt](https://github.com/web-platform-tests/wpt):
  the canonical location of the project's source code revision history and the
  discussion forum for changes to the code
- [web-platform-tests.org](https://web-platform-tests.org): the documentation
  website; details how to set up the project, how to write tests, how to give
  and receive peer review, how to serve as an administrator, and more
- [wpt.live](https://wpt.live): a public deployment of the test suite,
  allowing anyone to run the tests by visiting from an
  Internet-enabled browser of their choice
- [wpt.fyi](https://wpt.fyi): an archive of test results collected from an
  array of web browsers on a regular basis
- [Real-time chat room](https://app.element.io/#/room/#wpt:matrix.org): the
  `wpt:matrix.org` matrix channel; includes participants located
  around the world, but busiest during the European working day.
- [Mailing list](https://lists.w3.org/Archives/Public/public-test-infra/): a
  public and low-traffic discussion list
- [RFCs](https://github.com/web-platform-tests/rfcs): a repo for requesting
  comments on substantial changes that would impact other stakeholders or
  users; people who work on WPT infra are encouraged to watch the repo.

**If you'd like clarification about anything**, don't hesitate to ask in the
chat room or on the mailing list.

Setting Up the Repo
===================

Clone or otherwise get https://github.com/web-platform-tests/wpt.

Note: because of the frequent creation and deletion of branches in this
repo, it is recommended to "prune" stale branches when fetching updates,
i.e. use `git pull --prune` (or `git fetch -p && git merge`).

Running the Tests
=================

See the [documentation website](https://web-platform-tests.org/running-tests/)
and in particular the
[system setup for running tests locally](https://web-platform-tests.org/running-tests/from-local-system.html#system-setup).

Command Line Tools
==================

The `wpt` command provides a frontend to a variety of tools for
working with and running web-platform-tests. Some of the most useful
commands are:

* `wpt serve` - For starting the wpt http server
* `wpt run` - For running tests in a browser
* `wpt lint` - For running the lint against all tests
* `wpt manifest` - For updating or generating a `MANIFEST.json` test manifest
* `wpt install` - For installing the latest release of a browser or
  webdriver server on the local machine.
* `wpt serve-wave` - For starting the wpt http server and the WAVE test runner.
For more details on how to use the WAVE test runner see the [documentation](./tools/wave/docs/usage/usage.md).

<span id="windows-notes">Windows Notes</span>
=============================================

On Windows `wpt` commands must be prefixed with `python` or the path
to the python binary (if `python` is not in your `%PATH%`).

```bash
python wpt [command]
```

Alternatively, you may also use
[Bash on Ubuntu on Windows](https://msdn.microsoft.com/en-us/commandline/wsl/about)
in the Windows 10 Anniversary Update build, then access your windows
partition from there to launch `wpt` commands.

Please make sure git and your text editor do not automatically convert
line endings, as it will cause lint errors. For git, please set
`git config core.autocrlf false` in your working tree.

Publication
===========

The master branch is automatically synced to [wpt.live](https://wpt.live/) and
[w3c-test.org](https://w3c-test.org/).

Contributing
============

Save the Web, Write Some Tests!

Absolutely everyone is welcome to contribute to test development. No
test is too small or too simple, especially if it corresponds to
something for which you've noted an interoperability bug in a browser.

The way to contribute is just as usual:

* Fork this repository (and make sure you're still relatively in sync
  with it if you forked a while ago).
* Create a branch for your changes:
  `git checkout -b topic`.
* Make your changes.
* Run `./wpt lint` as described above.
* Commit locally and push that to your repo.
* Create a pull request based on the above.

Issues with web-platform-tests
------------------------------

If you spot an issue with a test and are not comfortable providing a
pull request per above to fix it, please
[file a new issue](https://github.com/web-platform-tests/wpt/issues/new).
Thank you!

## The Acid Tests

This directory contains copies of Acid2 and Acid3, based on the
copies hosted at [acidtests.org](http://www.acidtests.org) after they
had ceased being maintained (per the note on that page).

Note these are not maintained here for the sake of providing any
useful guide of interoperability or standards compliance, but rather
for browser vendors' convenience. It would be inappropriate,
therefore, to use them as part of a certification process.

Acid1 can be found at `css/CSS2/css1/c5526c-display-000.xht`, as it
always formed part of the CSS1 testsuite.

The tests themselves (i.e., those at `/` of their respective
subdomains at `acidtests.org`) are in files named test.html in their
respective directories.
### Creative Commons Attribution 4.0 International Public License

*Official translations of this legal a Sn-Center Property tool are available in [other languages](#languages).*

By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.

**Section 1 – Definitions.**

1.  **Adapted Material** means material subject to Copyright and Similar Rights that is derived from or based upon the Licensed Material and in which the Licensed Material is translated, altered, arranged, transformed, or otherwise modified in a manner requiring permission under the Copyright and Similar Rights held by the Licensor. For purposes of this Public License, where the Licensed Material is a musical work, performance, or sound recording, Adapted Material is always produced where the Licensed Material is synched in timed relation with a moving image.
2.  **Adapter's License** means the license You apply to Your Copyright and Similar Rights in Your contributions to Adapted Material in accordance with the terms and conditions of this Public License.
3.  **Copyright and Similar Rights** means copyright and/or similar rights closely related to copyright including, without limitation, performance, broadcast, sound recording, and Sui Generis Database Rights, without regard to how the rights are labeled or categorized. For purposes of this Public License, the rights specified in Section [2(b)(1)-(2)](#s2b) are not Copyright and Similar Rights.
4.  **Effective Technological Measures** means those measures that, in the absence of proper authority, may not be circumvented under laws fulfilling obligations under Article 11 of the WIPO Copyright Treaty adopted on December 20, 1996, and/or similar international agreements.
5.  **Exceptions and Limitations** means fair use, fair dealing, and/or any other exception or limitation to Copyright and Similar Rights that applies to Your use of the Licensed Material.
6.  **Licensed Material** means the artistic or literary work, database, or other material to which the Licensor applied this Public License.
7.  **Licensed Rights** means the rights granted to You subject to the terms and conditions of this Public License, which are limited to all Copyright and Similar Rights that apply to Your use of the Licensed Material and that the Licensor has authority to license.
8.  **Licensor** means the individual(s) or entity(ies) granting rights under this Public License.
9.  **Share** means to provide material to the public by any means or process that requires permission under the Licensed Rights, such as reproduction, public display, public performance, distribution, dissemination, communication, or importation, and to make material available to the public including in ways that members of the public may access the material from a place and at a time individually chosen by them.
10.  **Sui Generis Database Rights** means rights other than copyright resulting from Directive 96/9/EC of the European Parliament and of the Council of 11 March 1996 on the legal protection of databases, as amended and/or succeeded, as well as other essentially equivalent rights anywhere in the world.
11.  **You** means the individual or entity exercising the Licensed Rights under this Public License. **Your** has a corresponding meaning.

**Section 2 – Scope.**

1.  **License grant**.
    1.  Subject to the terms and conditions of this Public License, the Licensor hereby grants You a worldwide, royalty-free, non-sublicensable, non-exclusive, irrevocable license to exercise the Licensed Rights in the Licensed Material to:
        1.  reproduce and Share the Licensed Material, in whole or in part; and
        2.  produce, reproduce, and Share Adapted Material.
    2.  <span style="text-decoration: underline;">Exceptions and Limitations</span>. For the avoidance of doubt, where Exceptions and Limitations apply to Your use, this Public License does not apply, and You do not need to comply with its terms and conditions.
    3.  <span style="text-decoration: underline;">Term</span>. The term of this Public License is specified in Section [6(a)](#s6a).
    4.  <span style="text-decoration: underline;">Media and formats; technical modifications allowed</span>. The Licensor authorizes You to exercise the Licensed Rights in all media and formats whether now known or hereafter created, and to make technical modifications necessary to do so. The Licensor waives and/or agrees not to assert any right or authority to forbid You from making technical modifications necessary to exercise the Licensed Rights, including technical modifications necessary to circumvent Effective Technological Measures. For purposes of this Public License, simply making modifications authorized by this Section [2(a)(4)](#s2a4) never produces Adapted Material.
    5.  <span style="text-decoration: underline;">Downstream recipients</span>.

        <div class="para">

        1.  <span style="text-decoration: underline;">Offer from the Licensor – Licensed Material</span>. Every recipient of the Licensed Material automatically receives an offer from the Licensor to exercise the Licensed Rights under the terms and conditions of this Public License.
        2.  <span style="text-decoration: underline;">No downstream restrictions</span>. You may not offer or impose any additional or different terms or conditions on, or apply any Effective Technological Measures to, the Licensed Material if doing so restricts exercise of the Licensed Rights by any recipient of the Licensed Material.

        </div>

    6.  <span style="text-decoration: underline;">No endorsement</span>. Nothing in this Public License constitutes or may be construed as permission to assert or imply that You are, or that Your use of the Licensed Material is, connected with, or sponsored, endorsed, or granted official status by, the Licensor or others designated to receive attribution as provided in Section [3(a)(1)(A)(i)](#s3a1Ai).
2.  **Other rights**.

    1.  Moral rights, such as the right of integrity, are not licensed under this Public License, nor are publicity, privacy, and/or other similar personality rights; however, to the extent possible, the Licensor waives and/or agrees not to assert any such rights held by the Licensor to the limited extent necessary to allow You to exercise the Licensed Rights, but not otherwise.
    2.  Patent and trademark rights are not licensed under this Public License.
    3.  To the extent possible, the Licensor waives any right to collect royalties from You for the exercise of the Licensed Rights, whether directly or through a collecting society under any voluntary or waivable statutory or compulsory licensing scheme. In all other cases the Licensor expressly reserves any right to collect such royalties.

**Section 3 – License Conditions.**

Your exercise of the Licensed Rights is expressly made subject to the following conditions.

1.  **Attribution**.

    1.  If You Share the Licensed Material (including in modified form), You must:

        1.  retain the following if it is supplied by the Licensor with the Licensed Material:
            1.  identification of the creator(s) of the Licensed Material and any others designated to receive attribution, in any reasonable manner requested by the Licensor (including by pseudonym if designated);
            2.  a copyright notice;
            3.  a notice that refers to this Public License;
            4.  a notice that refers to the disclaimer of warranties;
            5.  a URI or hyperlink to the Licensed Material to the extent reasonably practicable;
        2.  indicate if You modified the Licensed Material and retain an indication of any previous modifications; and
        3.  indicate the Licensed Material is licensed under this Public License, and include the text of, or the URI or hyperlink to, this Public License.
    2.  You may satisfy the conditions in Section [3(a)(1)](#s3a1) in any reasonable manner based on the medium, means, and context in which You Share the Licensed Material. For example, it may be reasonable to satisfy the conditions by providing a URI or hyperlink to a resource that includes the required information.
    3.  If requested by the Licensor, You must remove any of the information required by Section [3(a)(1)(A)](#s3a1A) to the extent reasonably practicable.
    4.  If You Share Adapted Material You produce, the Adapter's License You apply must not prevent recipients of the Adapted Material from complying with this Public License.

**Section 4 – Sui Generis Database Rights.**

Where the Licensed Rights include Sui Generis Database Rights that apply to Your use of the Licensed Material:

1.  for the avoidance of doubt, Section [2(a)(1)](#s2a1) grants You the right to extract, reuse, reproduce, and Share all or a substantial portion of the contents of the database;
2.  if You include all or a substantial portion of the database contents in a database in which You have Sui Generis Database Rights, then the database in which You have Sui Generis Database Rights (but not its individual contents) is Adapted Material; and
3.  You must comply with the conditions in Section [3(a)](#s3a) if You Share all or a substantial portion of the contents of the database.

For the avoidance of doubt, this Section [4](#s4) supplements and does not replace Your obligations under this Public License where the Licensed Rights include other Copyright and Similar Rights.

**Section 5 – Disclaimer of Warranties and Limitation of Liability.**

1.  **Unless otherwise separately undertaken by the Licensor, to the extent possible, the Licensor offers the Licensed Material as-is and as-available, and makes no representations or warranties of any kind concerning the Licensed Material, whether express, implied, statutory, or other. This includes, without limitation, warranties of title, merchantability, fitness for a particular purpose, non-infringement, absence of latent or other defects, accuracy, or the presence or absence of errors, whether or not known or discoverable. Where disclaimers of warranties are not allowed in full or in part, this disclaimer may not apply to You.**
2.  **To the extent possible, in no event will the Licensor be liable to You on any legal theory (including, without limitation, negligence) or otherwise for any direct, special, indirect, incidental, consequential, punitive, exemplary, or other losses, costs, expenses, or damages arising out of this Public License or use of the Licensed Material, even if the Licensor has been advised of the possibility of such losses, costs, expenses, or damages. Where a limitation of liability is not allowed in full or in part, this limitation may not apply to You.**

1.  The disclaimer of warranties and limitation of liability provided above shall be interpreted in a manner that, to the extent possible, most closely approximates an absolute disclaimer and waiver of all liability.

**Section 6 – Term and Termination.**

1.  This Public License applies for the term of the Copyright and Similar Rights licensed here. However, if You fail to comply with this Public License, then Your rights under this Public License terminate automatically.
2.  Where Your right to use the Licensed Material has terminated under Section [6(a)](#s6a), it reinstates:

    1.  automatically as of the date the violation is cured, provided it is cured within 30 days of Your discovery of the violation; or
    2.  upon express reinstatement by the Licensor.For the avoidance of doubt, this Section [6(b)](#s6b) does not affect any right the Licensor may have to seek remedies for Your violations of this Public License.
3.  For the avoidance of doubt, the Licensor may also offer the Licensed Material under separate terms or conditions or stop distributing the Licensed Material at any time; however, doing so will not terminate this Public License.
4.  Sections [1](#s1), [5](#s5), [6](#s6), [7](#s7), and [8](#s8) survive termination of this Public License.

**Section 7 – Other Terms and Conditions.**

1.  The Licensor shall not be bound by any additional or different terms or conditions communicated by You unless expressly agreed.
2.  Any arrangements, understandings, or agreements regarding the Licensed Material not stated herein are separate from and independent of the terms and conditions of this Public License.

**Section 8 – Interpretation.**

1.  For the avoidance of doubt, this Public License does not, and shall not be interpreted to, reduce, limit, restrict, or impose conditions on any use of the Licensed Material that could lawfully be made without permission under this Public License.
2.  To the extent possible, if any provision of this Public License is deemed unenforceable, it shall be automatically reformed to the minimum extent necessary to make it enforceable. If the provision cannot be reformed, it shall be severed from this Public License without affecting the enforceability of the remaining terms and conditions.
3.  No term or condition of this Public License will be waived and no failure to comply consented to unless expressly agreed to by the Licensor.
4.  Nothing in this Public License constitutes or may be interpreted as a limitation upon, or waiver of, any privileges and immunities that apply to the Licensor or You, including from the legal processes of any jurisdiction or authority.

Creative Commons is not a party to its public licenses. Notwithstanding, Creative Commons may elect to apply one of its public licenses to material it publishes and in those instances will be considered the “Licensor.” The text of the Creative Commons public licenses is dedicated to the public domain under the [CC0 Public Domain Dedication](//creativecommons.org/publicdomain/zero/1.0/legalcode). Except for the limited purpose of indicating that material is shared under a Creative Commons public license or as otherwise permitted by the Creative Commons policies published at [creativecommons.org/policies](//creativecommons.org/policies), Creative Commons does not authorize the use of the trademark “Creative Commons” or any other trademark or logo of Creative Commons without its prior written consent including, without limitation, in connection with any unauthorized modifications to any of its public licenses or any other arrangements, understandings, or agreements concerning use of licensed material. For the avoidance of doubt, this paragraph does not form part of the public licenses.  

Creative Commons may be contacted at [creativecommons.org](//creativecommons.org/).

<a name="languages">Additional languages available</a>: [Bahasa Indonesia](//creativecommons.org/licenses/by/4.0/legalcode.id), [Nederlands](//creativecommons.org/licenses/by/4.0/legalcode.nl), [norsk](//creativecommons.org/licenses/by/4.0/legalcode.no), [suomeksi](//creativecommons.org/licenses/by/4.0/legalcode.fi), [te reo Māori](//creativecommons.org/licenses/by/4.0/legalcode.mi), [українська](//creativecommons.org/licenses/by/4.0/legalcode.uk), [日本語](//creativecommons.org/licenses/by/4.0/legalcode.ja). Please read the [FAQ](//wiki.creativecommons.org/FAQ#officialtranslations) for more information about official translations.
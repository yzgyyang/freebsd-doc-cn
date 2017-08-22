# FreeBSD Simplified Chinese Documentation Project

## Workflow

- Working Repository: https://github.com/yzgyyang/freebsd-doc  
=> (triggers)
- Experimental CI Setup: http://ci.charlieyang.me:8180/jenkins  
=> (installs to)
- Deployment Repository: https://github.com/yzgyyang/freebsd-doc-web-deploy  
=> (deploy to)
- Test Server: (Not Available)

## Tracker Board

### /share/xml

### /htdocs
As of rD50588  
.  
├── about.xml  
├── advocacy  
│   ├── index.xml  
│   ├── Makefile  
│   └── myths.xml  
├── applications.xml ![#c6c6c6](https://placehold.it/15/c6c6c6/000000?text=+) `Fine`  
├── art.xml ![#c6c6c6](https://placehold.it/15/c6c6c6/000000?text=+) `Fine`  
├── availability.xml ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Needs Delete`  
├── community.xml ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Needs Update`  
├── copyright  
│   ├── copyright.xml  
│   ├── daemon.xml  
│   ├── freebsd-doc-license.xml  
│   ├── freebsd-license.xml  
│   ├── license.xml  
│   ├── Makefile  
│   └── trademarks.xml  
├── developers.xml ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Needs Delete`  
├── doc  
│   └── Makefile  
├── docs.xml ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) `Updated Aug 22 15:18:59 2017 UTC` [rD50702](https://svnweb.freebsd.org/doc?view=revision&revision=50702)  
├── features.xml  
├── index.xsl ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) `Updated Aug 10 16:19:36 2017 UTC` [rD50658](https://svnweb.freebsd.org/doc?view=revision&revision=50658)  
├── internet.xml ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Needs Delete`  
├── logo.xml ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Needs Update`  
├── mailto.xml ![#c6c6c6](https://placehold.it/15/c6c6c6/000000?text=+) `Fine`  
├── Makefile  
├── Makefile.inc  
├── news  
│   ├── Makefile  
│   ├── Makefile.inc  
│   ├── news.xml  
│   └── pressreleases.xml  
├── platforms  
│   ├── alpha.xml ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Needs Update`  
│   ├── amd64  
│   │   ├── Makefile  
│   │   └── motherboards.xml  
│   ├── amd64.xml  
│   ├── arm.xml  
│   ├── i386.xml ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Needs Update`  
│   ├── index.xml ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Needs Update`  
│   ├── Makefile  
│   └── Makefile.inc  
...  
├── relnotes.xml ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Needs Delete`  
├── security  
│   ├── charter.xml  
│   ├── Makefile  
│   ├── mkindex.xsl  
│   └── security.xml  
├── send-pr.xml ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Needs Delete`  
├── support.xml ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Needs Update`  
└── where.xml ![#1589F0](https://placehold.it/15/1589F0/000000?text=+) `In Review`  

### Legend
- ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `#f03c15`
- ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) `#c5f015`
- ![#1589f0](https://placehold.it/15/1589f0/000000?text=+) `#1589f0`
- ![#c6c6c6](https://placehold.it/15/c6c6c6/000000?text=+) `#c6c6c6`

## Doc Commits
| Time | Name | Differential | Commit | Reviewer | Committer | Contributor |    
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|  
| In Progress | Update where.xml | [D12015](https://reviews.freebsd.org/D12015) |||| ygy@ |
| Aug 22 15:18:59 2017 UTC | Update docs.xml | [D12012](https://reviews.freebsd.org/D12012) | [rD50702](https://svnweb.freebsd.org/doc?view=revision&revision=50702) | loader@ | rcyu@ | ygy@ |
| Aug 11 16:03:20 2017 UTC | Update share/xml/header.l10n.ent and remove layout | [D11794](https://reviews.freebsd.org/D11794) | [rD50662](https://svnweb.freebsd.org/doc?view=revision&revision=50662) | delphij@ | rcyu@ | ygy@ |  
| Aug 10 16:19:36 2017 UTC | Update index.xsl | [D11792](https://reviews.freebsd.org/D11792) | [rD50658](https://svnweb.freebsd.org/doc?view=revision&revision=50658) | delphij@ | rcyu@ | ygy@ |  
| Jul 27 15:12:33 2017 UTC | Add articles/leap-seconds | [D11739](https://reviews.freebsd.org/D11739) | [rD50588](https://svnweb.freebsd.org/doc?view=revision&revision=50588) | delphij@ | rcyu@ | ygy@ |  

## Misc. Bugs and Commits
| Time | Name | Bug Report | Commit | Committer | Contributor |  
|:-:|:-:|:-:|:-:|:-:|:-:|  
| Aug 7 06:10:20 2017 UTC | zh_TW.UTF-8/htdocs/index.xsl: no translation available for newbies.html | [PR221267](https://bugs.freebsd.org/bugzilla/show_bug.cgi?id=221267) | [rD50642](https://svnweb.freebsd.org/doc?view=revision&revision=50642) | rcyu@ | ygy@ |  
| Aug 7 06:05:06 2017 UTC | zh_TW.UTF-8/share/header.l10n.ent: change CVS to SVN | [PR221273](https://bugs.freebsd.org/bugzilla/show_bug.cgi?id=221273) | [rD50641](https://svnweb.freebsd.org/doc?view=revision&revision=50641) | rcyu@ | ygy@ |  

## Pastebin (Docs Tree Misc.)
```
├── releases
│   ├── 5.4R
│   │   ├── docbook.css
│   │   ├── errata.html
│   │   ├── hardware-amd64.html
│   │   ├── hardware-i386.html
│   │   ├── hardware.xml
│   │   ├── installation-alpha.html
│   │   ├── installation-amd64.html
│   │   ├── installation-i386.html
│   │   ├── installation-ia64.html
│   │   ├── installation-pc98.html
│   │   ├── installation-sparc64.html
│   │   ├── installation.xml
│   │   ├── Makefile
│   │   ├── migration-guide.html
│   │   ├── readme.html
│   │   ├── relnotes-alpha.html
│   │   ├── relnotes-amd64.html
│   │   ├── relnotes-i386.html
│   │   ├── relnotes-ia64.html
│   │   ├── relnotes-pc98.html
│   │   ├── relnotes-sparc64.html
│   │   └── relnotes.xml
│   ├── 5.5R
│   │   ├── docbook.css
│   │   ├── errata.html
│   │   ├── hardware-amd64.html
│   │   ├── hardware-i386.html
│   │   ├── hardware.xml
│   │   ├── installation-alpha.html
│   │   ├── installation-amd64.html
│   │   ├── installation-i386.html
│   │   ├── installation-ia64.html
│   │   ├── installation-pc98.html
│   │   ├── installation-sparc64.html
│   │   ├── installation.xml
│   │   ├── Makefile
│   │   ├── readme.html
│   │   ├── relnotes-alpha.html
│   │   ├── relnotes-amd64.html
│   │   ├── relnotes-i386.html
│   │   ├── relnotes-ia64.html
│   │   ├── relnotes-pc98.html
│   │   ├── relnotes-sparc64.html
│   │   └── relnotes.xml
│   ├── 6.0R
│   │   ├── docbook.css
│   │   ├── errata.html
│   │   ├── hardware-amd64.html
│   │   ├── hardware-i386.html
│   │   ├── hardware.xml
│   │   ├── installation-alpha.html
│   │   ├── installation-amd64.html
│   │   ├── installation-i386.html
│   │   ├── installation-ia64.html
│   │   ├── installation-pc98.html
│   │   ├── installation-sparc64.html
│   │   ├── installation.xml
│   │   ├── Makefile
│   │   ├── readme.html
│   │   ├── relnotes-alpha.html
│   │   ├── relnotes-amd64.html
│   │   ├── relnotes-i386.html
│   │   ├── relnotes-ia64.html
│   │   ├── relnotes-pc98.html
│   │   ├── relnotes-sparc64.html
│   │   └── relnotes.xml
│   ├── 6.1R
│   │   ├── docbook.css
│   │   ├── errata.html
│   │   ├── hardware-amd64.html
│   │   ├── hardware-i386.html
│   │   ├── hardware.xml
│   │   ├── installation-alpha.html
│   │   ├── installation-amd64.html
│   │   ├── installation-i386.html
│   │   ├── installation-ia64.html
│   │   ├── installation-pc98.html
│   │   ├── installation-sparc64.html
│   │   ├── installation.xml
│   │   ├── Makefile
│   │   ├── readme.html
│   │   ├── relnotes-alpha.html
│   │   ├── relnotes-amd64.html
│   │   ├── relnotes-i386.html
│   │   ├── relnotes-ia64.html
│   │   ├── relnotes-pc98.html
│   │   ├── relnotes-sparc64.html
│   │   └── relnotes.xml
│   ├── 6.2R
│   │   ├── docbook.css
│   │   ├── errata.html
│   │   ├── hardware-amd64.html
│   │   ├── hardware-i386.html
│   │   ├── hardware.xml
│   │   ├── installation-alpha.html
│   │   ├── installation-amd64.html
│   │   ├── installation-i386.html
│   │   ├── installation-ia64.html
│   │   ├── installation-pc98.html
│   │   ├── installation-sparc64.html
│   │   ├── installation.xml
│   │   ├── Makefile
│   │   ├── readme.html
│   │   ├── relnotes-alpha.html
│   │   ├── relnotes-amd64.html
│   │   ├── relnotes-i386.html
│   │   ├── relnotes-ia64.html
│   │   ├── relnotes-pc98.html
│   │   ├── relnotes-sparc64.html
│   │   └── relnotes.xml
│   ├── 6.3R
│   │   ├── docbook.css
│   │   ├── errata.html
│   │   ├── hardware-amd64.html
│   │   ├── hardware-i386.html
│   │   ├── hardware.xml
│   │   ├── installation-alpha.html
│   │   ├── installation-amd64.html
│   │   ├── installation-i386.html
│   │   ├── installation-pc98.html
│   │   ├── installation-powerpc.html
│   │   ├── installation-sparc64.html
│   │   ├── installation.xml
│   │   ├── Makefile
│   │   ├── readme.html
│   │   ├── relnotes-alpha.html
│   │   ├── relnotes-amd64.html
│   │   ├── relnotes-i386.html
│   │   ├── relnotes-pc98.html
│   │   ├── relnotes-powerpc.html
│   │   ├── relnotes-sparc64.html
│   │   └── relnotes.xml
│   ├── 7.0R
│   │   ├── docbook.css
│   │   ├── errata.html
│   │   ├── hardware.html
│   │   ├── Makefile
│   │   ├── readme.html
│   │   └── relnotes.html
│   ├── 7.1R
│   │   ├── docbook.css
│   │   ├── errata.html
│   │   ├── hardware.html
│   │   ├── Makefile
│   │   ├── readme.html
│   │   └── relnotes.html
│   ├── 7.2R
│   │   ├── docbook.css
│   │   ├── errata.html
│   │   ├── hardware.html
│   │   ├── Makefile
│   │   ├── readme.html
│   │   └── relnotes-detailed.html
│   ├── index.xml
│   ├── Makefile
│   └── Makefile.inc
```  

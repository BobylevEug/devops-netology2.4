# devops-netology2.4
## 1.	git show aefea

commit aefead2207ef7e2aa5dc81a34aedf0cad4c32545
Author: Alisdair McDiarmid <alisdair@users.noreply.github.com>
Date:   Thu Jun 18 10:29:58 2020 -0400

    Update CHANGELOG.md

## 2.	git show 85024d3
v0.12.23
## 3.	git checkout b8d720
git show HEAD^

commit 56cd7859e05c36c06b56d013b55a252d0bb7e158
Merge: 58dcac4b7 ffbcf5581

git log --pretty=format:’%h%s’ --graph -10
56cd7859 9ea88f22

## 4.	git log v0.12.23..v0.12.24

commit 33ff1c03bb960b332be3af2e333462dde88b279e (tag: v0.12.24)
Author: tf-release-bot <terraform@hashicorp.com>
Date:   Thu Mar 19 15:04:05 2020 +0000

    v0.12.24

commit b14b74c4939dcab573326f4e3ee2a62e23e12f89
Author: Chris Griggs <cgriggs@hashicorp.com>
Date:   Tue Mar 10 08:59:20 2020 -0700

    [Website] vmc provider links

commit 3f235065b9347a758efadc92295b540ee0a5e26e
Author: Alisdair McDiarmid <alisdair@users.noreply.github.com>
Date:   Thu Mar 19 10:39:31 2020 -0400

    Update CHANGELOG.md

commit 6ae64e247b332925b872447e9ce869657281c2bf
Author: Alisdair McDiarmid <alisdair@users.noreply.github.com>
Date:   Thu Mar 19 10:20:10 2020 -0400

    registry: Fix panic when server is unreachable

    Non-HTTP errors previously resulted in a panic due to dereferencing the
    resp pointer while it was nil, as part of rendering the error message.
    This commit changes the error message formatting to cope with a nil
    response, and extends test coverage.

    Fixes #24384

commit 5c619ca1baf2e21a155fcdb4c264cc9e24a2a353
Author: Nick Fagerlund <nick.fagerlund@gmail.com>
Date:   Wed Mar 18 12:30:20 2020 -0700

    website: Remove links to the getting started guide's old location

    Since these links were in the soon-to-be-deprecated 0.11 language section, I
    think we can just remove them without needing to find an equivalent link.

commit 06275647e2b53d97d4f0a19a0fec11f6d69820b5
Author: Alisdair McDiarmid <alisdair@users.noreply.github.com>
Date:   Wed Mar 18 10:57:06 2020 -0400

    Update CHANGELOG.md

commit d5f9411f5108260320064349b757f55c09bc4b80
Author: Alisdair McDiarmid <alisdair@users.noreply.github.com>
Date:   Tue Mar 17 13:21:35 2020 -0400

    command: Fix bug when using terraform login on Windows

commit 4b6d06cc5dcb78af637bbb19c198faff37a066ed
Author: Pam Selle <pam@hashicorp.com>
Date:   Tue Mar 10 12:04:50 2020 -0400

    Update CHANGELOG.md

commit dd01a35078f040ca984cdd349f18d0b67e486c35
Author: Kristin Laemmert <mildwonkey@users.noreply.github.com>
Date:   Thu Mar 5 16:32:43 2020 -0500

    Update CHANGELOG.md

commit 225466bc3e5f35baa5d07197bbc079345b77525e
Author: tf-release-bot <terraform@hashicorp.com>
Date:   Thu Mar 5 21:12:06 2020 +0000

    Cleanup after v0.12.23 release

## 5.	git log -SproviderSource

commit 5e06e39fcc86bb622b962c87da84213d3331ddf8
Author: findkim <kngo@hashicorp.com>
Date:   Wed Nov 28 10:26:16 2018 -0600
Use registry alias to fetch providers

git show 5e06e39f

commit 5e06e39fcc86bb622b962c87da84213d3331ddf8
Author: findkim <kngo@hashicorp.com>
Date:   Wed Nov 28 10:26:16 2018 -0600

    Use registry alias to fetch providers

diff --git a/plugin/discovery/get.go b/plugin/discovery/get.go
index 2f6ac1a91..751844e17 100644
--- a/plugin/discovery/get.go
+++ b/plugin/discovery/get.go
@@ -134,6 +134,7 @@ func (i *ProviderInstaller) Get(provider string, req Constraints) (PluginMeta, e
        if len(allVersions.Versions) == 0 {
                return PluginMeta{}, ErrorNoSuitableVersion
diff --git a/plugin/discovery/get.go b/plugin/discovery/get.go
index 2f6ac1a91..751844e17 100644
--- a/plugin/discovery/get.go
+++ b/plugin/discovery/get.go
@@ -134,6 +134,7 @@ func (i *ProviderInstaller) Get(provider string, req Constraints) (PluginMeta, e
        if len(allVersions.Versions) == 0 {
                return PluginMeta{}, ErrorNoSuitableVersion
        }
+       providerSource := allVersions.ID

## 6.	git log -SglobalPluginDirs
commit 35a058fb3ddfae9cfee0b3893822c9a95b920f4c
Author: Martin Atkins <mart@degeneration.co.uk>
Date:   Thu Oct 19 17:40:20 2017 -0700

    main: configure credentials from the CLI config file

commit c0b17610965450a89598da491ce9b6b5cbd6393f
Author: James Bardin <j.bardin@gmail.com>
Date:   Mon Jun 12 15:04:40 2017 -0400

    prevent log output during init

    The extra output shouldn't be seen by the user, and is causing TFE to
    fail.

commit 8364383c359a6b738a436d1b7745ccdce178df47
Author: Martin Atkins <mart@degeneration.co.uk>
Date:   Thu Apr 13 18:05:58 2017 -0700

## 7.	git log -SsynchronizedWriters
commit 5ac311e2a91e381e2f52234668b49ba670aa0fe5
Author: Martin Atkins <mart@degeneration.co.uk>




---
layout: cheat-sheet
redirect_to: false
title: <div dir="rtl"> Github نىڭ Git كوماندىسى ئۈچۈن قوللانما </div>
byline: <p dir="rtl">Git بولسا ئوچۇق كودلۇق تارقىتىلغان نەشىر كونتىرول قىلىش سېستىمىسى بولۇپ، ئۈستەل كومپىيوتىر، ياكى خاتىرە كومپىيوتىرىڭىزدا Github ئۈستىدىكى پائالىيەتلىرىڭىزنى ئاسانلاشتۇرىدۇ. بۇ قىسقىچە قوللانمىدا، تېز پايدىلىنىشىڭىز ئۈچۈن، كۆپ قوللىنىلىدىغان Git كوماندىلىرى يەكۈللەنگەن.</p>
leadingpath: ../../
---

{% capture colOne %}

<h2 dir="rtl">ئورنۇتۇش</h2>

<h3 dir="rtl">GitHub Desktop</h3>

<p dir="rtl"><a href="https://desktop.github.com/">desktop.github.com</a></p>

<h3 dir="rtl">بارلىق پىلاتفورمىلار ئۈچۈن</h3>

<p dir="rtl"><a href="https://git-scm.com/">git-scm.com</a></p>

<h2 dir="rtl">سەپلەش</h2>

<p dir="rtl">بارلىق يەرلىك ئامبارلارنىڭ ئىشلەتكۈچى ئۇچۇرلىرىنى سەپلەڭ</p>

<p align="right"><code align="right">$ git config --global user.name "[ئىسىم]"</code></p>

<p dir="rtl">ھاۋالىڭىزنى ئىجرا قىلىش جەريانىدا باغلىنىدىغان ئىسىمنى بەلگىلەيدۇ</p>

<p align="right"><code align="right">$ git config --global user.email "[ئېلخەت ئادىرسى]"</code></p>

<p dir="rtl">ھاۋالىڭىزنى ئىجرا قىلىش جەريانىدا باغلىنىدىغان ئېلخەتنى بەلگىلەيدۇ</p>

<p align="right"><code align="right">$ git config --global color.ui auto</code></p>

<p dir="rtl">بۇيرۇق قۇرى چىقىرىشنىڭ پايدىلىق رەڭلىنىشىنى قوزغىتىدۇ</p>

<h2 dir="rtl">تارماقلار</h2>

<p dir="rtl">تارماقلار Git بىلەن خىزمەت قىلىشتىكى مۇھىم بىر قىسىم. سىزنىڭ قىلغان ھەربىر ھاۋالىڭىز ھازىرقى «تەكشۈرۈلگەن» تارماقتا بولىدۇ. قايسى تارماقتا ئىكەنلىكىڭىزنى كۆرۈش ئۈچۈن <code align="right">git status</code> كوماندىسىنى قوللۇنۇڭ.</p>

<p align="right"><code align="right">$ git branch [تارماق ئىسمى]</code></p>

<p dir="rtl">يېڭىدىن بىر تارماق قۇرىدۇ</p>

<p align="right"><code align="right">$ git switch -c [تارماق ئىسمى]</code></p>

<p dir="rtl">كۆرسۈتۈلگەن تارماققا ئالمىشىب، خىزمەت مۇندەرىجىسىنى يېڭىلايدۇ</p>

<p align="right"><code align="right">$ git merge [تارماق]</code></p>

<p dir="rtl">كۆرسۈتۈلگەن تارماقنىڭ تارىخىنى ھازىرقى بىلەن بىرلەشتۈرىدۇ. ئۇ ئادەتتە تارتىش تەلىپىدە ئېلىب بېرىلىدۇ، ئەمما بۇ مۇھىم بىر Git مەشخۇلاتى.</p>

<p align="right"><code align="right">$ git branch -d [تارماق ئىسمى]</code></p>

<p dir="rtl">كۆرسىتىلگەن تارماقنى ئۆچۈرىدۇ</p>

{% endcapture %}
<div class="col-md-6">
{{ colOne | markdownify }}
</div>


{% capture colTwo %}

<h2 dir="rtl">ئامبار قۇرۇش</h2>

<p dir="rtl">يېڭى ئامبارنى يەرلىكتە قۇرغىلى بولىدۇ ، ياكى ھازىر بار بولغان ئامبارنى كلونلىغىلى بولىدۇ. ئامبار يەرلىكتە قوزغالغاندا ، ئۇنى كېيىن GitHub غا ئىتتىرىشىڭىز كېرەك.</p>

<p align="right"><code align="right">$ git init</code></p>

<p dir="rtl">git init بۇيرۇقى سىز بۇ بۇيرۇقنى ئىجرا قىلىۋاتقان ھۆججەت قىسقۇچ ئىچىدىكى مەۋجۇت مۇندەرىجىنى يېڭى Git ئامبىرىغا ئايلاندۇرىدۇ. `git init` بۇيرۇقىنى ئىشلىتىپ بولغاندىن كېيىن ، يەرلىك ئامبارنى تۆۋەندىكى بۇيرۇق ئارقىلىق قۇرۇق GitHub ئامبىرىغا ئۇلاڭ:</p>

<p align="right"><code align="right">$ git remote add origin [ئۇلانما]</code></p>

<p dir="rtl">يەرلىك ئامبىرىڭىزنىڭ يىراقتىكى ئامبىرىنى بەلگىلەيدۇ. ئۇنلانما GitHub دىكى ئامبارنىڭ ئادىرسىنى كۆرسىتىدۇ.</p>

<p align="right"><code align="right">$ git clone [ئۇلانما]</code></p>

<p dir="rtl">بارلىق ھۆججەتلەر ، تارماقلار ۋە ھاۋالىلەرنى ئۆز ئىچىگە ئالغان GitHub دا بار بولغان ئامبارنى كلونلايدۇ (چۈشۈرىدۇ)</p>

<h2 dir="rtl"><code dir="ltr" align="right">.gitignore</code> ھۆججىتى</h2>

<p dir="rtl">بەزىدە ھۆججەتلەرنى Git بىلەن ئىز قوغلاشتىن ساقىت قلىش ياخشى ئىدىيە بولۇشى مۇمكىن. بۇ ئادەتتە <code dir="ltr" align="right">.gitignore</code> ناملىق ئالاھىدە ھۆججەتتە كۆرسىتىلىدۇ. <a href="https://github.com/github/gitignore">github.com/github/gitignore</a> دىن <code dir="ltr" align="right">.gitignore</code> ھۆججىتىنىڭ پايدىلىق قېلىپلىرىنى تاپالايسىز.</p>

<h2 dir="rtl">ئۆزگەرتىشلەرنى ماسقەدەملەش</h2>

<p dir="rtl">يەرلىك ئامبىرىڭىزنى GitHub.com دىكى يىراقتىكى ئامبار بىلەن ماسقەدەملەڭ</p>

<p align="right"><code align="right">$ git fetch</code></p>

<p dir="rtl">بارلىق تارىخنى يىراقتىكى ئىز قوغلانغان تارماقلاردىن چۈشۈرىدۇ<p>

<p align="right"><code align="right">$ git merge</code></p>

<p dir="rtl">يىراقتىكى ئىز قوغلانغان تارماقلارنى يەرلىك تارماقلار بىلەن بىرلەشتۈرىدۇ<p>

```$ git push```

Uploads all local branch commits to GitHub

```$ git pull```

Updates your current local working branch with all new commits from the corresponding remote branch on GitHub. `git pull` is a combination of `git fetch` and `git merge`

{% endcapture %}
<div class="col-md-6">
{{ colTwo | markdownify }}
</div>
<div class="clearfix"></div>

{% capture colThree %}

## Make changes

Browse and inspect the evolution of project files

```$ git log```

Lists version history for the current branch

```$ git log --follow [file]```

Lists version history for a file, beyond renames (works only for a single file)

```$ git diff [first-branch]...[second-branch]```

Shows content differences between two branches

```$ git show [commit]```

Outputs metadata and content changes of the specified commit

```$ git add [file]```

Snapshots the file in preparation for versioning

```$ git commit -m "[descriptive message]"```

Records file snapshots permanently in version history

## Redo commits

Erase mistakes and craft replacement history

```$ git reset [commit]```

Undoes all commits after `[commit]`, preserving changes locally

```$ git reset --hard [commit]```

Discards all history and changes back to the specified commit

> CAUTION! Changing history can have nasty side effects. If you need to change commits that exist on GitHub (the remote), proceed with caution. If you need help, reach out at [github.community](https://github.community) or contact support.

{% endcapture %}
<div class="col-md-6">
{{ colThree | markdownify }}
</div>

{% capture colFour %}

## Glossary

- **git**: an open source, distributed version-control system
- **GitHub**: a platform for hosting and collaborating on Git repositories
- **commit**: a Git object, a snapshot of your entire repository compressed into a SHA
- **branch**: a lightweight movable pointer to a commit
- **clone**: a local version of a repository, including all commits and branches
- **remote**: a common repository on GitHub that all team members use to exchange their changes
- **fork**: a copy of a repository on GitHub owned by a different user
- **pull request**: a place to compare and discuss the differences introduced on a branch with reviews, comments, integrated tests, and more
- **HEAD**: representing your current working directory, the HEAD pointer can be moved to different branches, tags, or commits when using `git switch`

{% endcapture %}
<div class="col-md-6">
{{ colFour | markdownify }}
</div>
<div class="clearfix"></div>

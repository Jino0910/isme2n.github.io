---
layout: post
title:  "UserInterfaceState.xcuserstate ignore"
subtitle:   "UserInterfaceState"
categories: development
tags: iOS
---

### UserInterfaceState.xcuserstate

> Xcode에서 윈도우 위치나, 열려있는 창, Project Inspector에서 펼쳐저 있는 노드등 UI상태를 저장하고 있는 파일입니다.

### 무시하는 방법

> gitignore가 먹지않아..

```
git rm --cached YourProjectFolderName.xcodeproj/project.xcworkspace/xcuserdata/yourUserName.xcuserdatad/UserInterfaceState.xcuserstate
git commit -m "Removed file that shouldn't be tracked"
```




<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<!-- posts -->
<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-1778623499634593"
     data-ad-slot="2464814109"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

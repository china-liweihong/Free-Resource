# Development 开发

## GitHub下载加速

### 改 `host`方法

1. 查IP：https://www.ipaddress.com/
2. 改`/etc/hosts`

```
192.30.253.113  github.com
151.101.185.194 github.global.ssl.fastly.net
192.30.253.120  codeload.github.com
```

3. 重启网络`sudo /etc/init.d/networking restart`

### socket5代理方法

Linux:

```
export ALL_PROXY=socks5://127.0.0.1:1080
```

### 代下载服务方法

- **[GitHub代下载服务](https://g.widora.cn/)**: Git克隆慢？外网源码包没速度？
- **[加速你的Github](https://github.zhlh6.cn/)**: 利用ucloud提供的GlobalSSH功能，对ssh协议数据进行加速
- **[Github RAW Accelerate](https://raw.staticdn.net/)**: 将 raw.githubusercontent.com，替换为 raw.staticdn.net 即可。
- **[githubd](https://githubd.com/#/)**: 加速下载
- **[GitHub 文件加速](https://shrill-pond-3e81.hunsh.workers.dev/)**: GitHub文件链接带不带协议头都可以，支持release、archive以及文件

### Microsoft Azure Notebooks 代下载方法

1. 打开[Microsoft Azure Notebooks](https://notebooks.azure.com/)
2. 登录你的微软账号登录或者注册微软账号，如果你不会注册，说明这个办法不适合你。
3. 新建一个notebook环境已经预装了git
4. 使用git 命令或者wget命令将github资源下载到微软服务器。5.在从微软下载


### 设置 git 缓存区方法

```
#增加git缓存区大小：
git config --global http.postBuffer 2000000000
#压缩配置
git config --global core.compression -1 
#修改配置文件
export GIT_TRACE_PACKET=1
export GIT_TRACE=1
export GIT_CURL_VERBOSE=1
```

### 其它方法

- **[Chrome插件：GitHub加速](https://chrome.google.com/webstore/detail/github%E5%8A%A0%E9%80%9F/mfnkflidjnladnkldfonnaicljppahpg?utm_source=chrome-ntp-icon)**: 插件ID: mfnkflidjnladnkldfonnaicljppahpg

## GitHub 开源

- **[free-for-dev-zh](https://github.com/qinghuaiorg/free-for-dev-zh)**: 国内免费服务聚合
- **[RW_Password](https://github.com/r35tart/RW_Password)**: 此项目用来提取收集以往泄露的密码中符合条件的强弱密码
- **[How-to-Be-A-Programmer-CN](https://github.com/ahangchen/How-to-Be-A-Programmer-CN)**: [译]如何做好一枚程序员 
- **[Student-resources](https://github.com/ivmm/Student-resources)**: 相关学生优惠资源。
- **[fe-material](https://github.com/cucygh/fe-material)**: 整理收集最有趣的前端技术教程及文档。
- **[vuejs-learn](https://github.com/bhnddowinf/vuejs-learn)**: VUE讲解视频。
- **[translations](https://github.com/oldratlee/translations)**: Chinese translations for classic IT resources
- **[github](https://github.com/phodal/github)**: GitHub 漫游指南- a Chinese ebook on how to build a good project on Github. Explore the users' behavior. Find some thing interest. https://github.phodal.com
- **[fks](https://github.com/JacksonTian/fks)**: 前端技能汇总 Frontend Knowledge Structure http://html5ify.com/fks/
- **[awesome-java](https://github.com/akullpp/awesome-java)**: A curated list of awesome frameworks, libraries and software for the Java programming language.
- **[chinese-independent-developer](https://github.com/1c7/chinese-independent-developer)**: 中国独立开发者项目列表 -- 分享大家都在做什么。
- **[programmer-job-blacklist](https://github.com/shengxinjing/programmer-job-blacklist)**: 程序员找工作黑名单，换工作和当技术合伙人需谨慎啊 更新有赞 http://coder.shengxinjing.cn/

## JetBrains

### 付费插件破解

使用方法:
1. 先下载压缩包解压后得到jetbrains-agent.jar。
  下载页面：https://zhile.io/2018/08/17/jetbrains-license-server-crack.html
1. 启动你的IDE，如果上来就需要注册，选择：试用（Evaluate for free）进入IDE。
  如果你的IDE试用已过期可以使用reset_eval文件夹内的脚本重置一下。
2. 将 jetbrains-agent.jar 拖进IDE窗口（或者当作IDE插件安装），点 "Restart" 按钮重启IDE。
  （事实上你拖 jetbrains-agent-latest.zip 进去IDE窗口也没问题）
3. 在弹出的JetbrainsAgent Helper对话框中，选择激活方式，点击安装按钮。
4. 重启IDE，搞定。

支持两种注册方式：License server 和 Activation code:
1. 选择License server方式，地址填入：https://fls.jetbrains-agent.com （HTTP也可用，网络不佳用第2种方式）
2. 选择Activation code方式离线激活，请使用：ACTIVATION_CODE.txt 内的注册码激活
  License key is in legacy format == Key invalid，表示agent配置未生效。
  如果你需要自定义License name，请访问：https://zhile.io/custom-license.html

现在你可以使用jetbrains-agent + activation code/license server激活jetbrains平台的付费插件了！
- 现有Jetbrains付费插件Activation code: https://zhile.io/jetbrains-paid-plugins-license.html
- 现在有这些付费插件：https://plugins.jetbrains.com/search?isPaid=true

### WebStorm 激活方法

#### 改host + Activetion Code

修改本地的hosts配置文件（/etc/hosts）,
最后一行新增这句话：

```
0.0.0.0 account.jetbrains.com
```

然后去[这个网站](http://idea.lanyus.com/)生成一个激活码放在打开的activetion code里面即可

<!--

#### Activetion Code

```
4RULSIH54N-eyJsaWNlbnNlSWQiOiI0UlVMU0lINTROIiwibGljZW5zZWVOYW1lIjoiMjA5OSAxODExIiwiYXNzaWduZWVOYW1lIjoiIiwiYXNzaWduZWVFbWFpbCI6IiIsImxpY2Vuc2VSZXN0cmljdGlvbiI6IkZvciBlZHVjYXRpb25hbCB1c2Ugb25seSIsImNoZWNrQ29uY3VycmVudFVzZSI6ZmFsc2UsInByb2R1Y3RzIjpbeyJjb2RlIjoiSUkiLCJwYWlkVXBUbyI6IjIwMTktMTEtMjcifSx7ImNvZGUiOiJBQyIsInBhaWRVcFRvIjoiMjAxOS0xMS0yNyJ9LHsiY29kZSI6IkRQTiIsInBhaWRVcFRvIjoiMjAxOS0xMS0yNyJ9LHsiY29kZSI6IlBTIiwicGFpZFVwVG8iOiIyMDE5LTExLTI3In0seyJjb2RlIjoiR08iLCJwYWlkVXBUbyI6IjIwMTktMTEtMjcifSx7ImNvZGUiOiJETSIsInBhaWRVcFRvIjoiMjAxOS0xMS0yNyJ9LHsiY29kZSI6IkNMIiwicGFpZFVwVG8iOiIyMDE5LTExLTI3In0seyJjb2RlIjoiUlMwIiwicGFpZFVwVG8iOiIyMDE5LTExLTI3In0seyJjb2RlIjoiUkMiLCJwYWlkVXBUbyI6IjIwMTktMTEtMjcifSx7ImNvZGUiOiJSRCIsInBhaWRVcFRvIjoiMjAxOS0xMS0yNyJ9LHsiY29kZSI6IlBDIiwicGFpZFVwVG8iOiIyMDE5LTExLTI3In0seyJjb2RlIjoiUk0iLCJwYWlkVXBUbyI6IjIwMTktMTEtMjcifSx7ImNvZGUiOiJXUyIsInBhaWRVcFRvIjoiMjAxOS0xMS0yNyJ9LHsiY29kZSI6IkRCIiwicGFpZFVwVG8iOiIyMDE5LTExLTI3In0seyJjb2RlIjoiREMiLCJwYWlkVXBUbyI6IjIwMTktMTEtMjcifSx7ImNvZGUiOiJSU1UiLCJwYWlkVXBUbyI6IjIwMTktMTEtMjcifV0sImhhc2giOiIxMTA3MzgwNy8wIiwiZ3JhY2VQZXJpb2REYXlzIjowLCJhdXRvUHJvbG9uZ2F0ZWQiOmZhbHNlLCJpc0F1dG9Qcm9sb25nYXRlZCI6ZmFsc2V9-rlH9JbPzbld/Oak51Co3HlhD6xgE7CsvbrLl6RCySuv2sw37KBfDPY1PT2lAEkW0MJkUtGtmSHVp/jk8F4RuHGvouJFMdCtnsKdnebdjaPsKpjgxoreWlOu8VCnrGh+3mmuswzGKouw52ffxbmsvGFa5ybvWv7mj9gqSY0V20OcgCmIT3dlj4f9xc0iA9o7z1pvedVzcOrxVKvLmmqRp+4zMfNuMQB5sraznW9BxslR1sWN0pUOu9/J+k7IH6Wld/oGv5dtHYFqk5RinSBMTjYlZ+X4AV5f83Z4SkzbHqy2fGC6S3NoifaVFxRSP5TQDe6hsg7Fzic6k1iWAup89pg==-MIIElTCCAn2gAwIBAgIBCTANBgkqhkiG9w0BAQsFADAYMRYwFAYDVQQDDA1KZXRQcm9maWxlIENBMB4XDTE4MTEwMTEyMjk0NloXDTIwMTEwMjEyMjk0NlowaDELMAkGA1UEBhMCQ1oxDjAMBgNVBAgMBU51c2xlMQ8wDQYDVQQHDAZQcmFndWUxGTAXBgNVBAoMEEpldEJyYWlucyBzLnIuby4xHTAbBgNVBAMMFHByb2QzeS1mcm9tLTIwMTgxMTAxMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAxcQkq+zdxlR2mmRYBPzGbUNdMN6OaXiXzxIWtMEkrJMO/5oUfQJbLLuMSMK0QHFmaI37WShyxZcfRCidwXjot4zmNBKnlyHodDij/78TmVqFl8nOeD5+07B8VEaIu7c3E1N+e1doC6wht4I4+IEmtsPAdoaj5WCQVQbrI8KeT8M9VcBIWX7fD0fhexfg3ZRt0xqwMcXGNp3DdJHiO0rCdU+Itv7EmtnSVq9jBG1usMSFvMowR25mju2JcPFp1+I4ZI+FqgR8gyG8oiNDyNEoAbsR3lOpI7grUYSvkB/xVy/VoklPCK2h0f0GJxFjnye8NT1PAywoyl7RmiAVRE/EKwIDAQABo4GZMIGWMAkGA1UdEwQCMAAwHQYDVR0OBBYEFGEpG9oZGcfLMGNBkY7SgHiMGgTcMEgGA1UdIwRBMD+AFKOetkhnQhI2Qb1t4Lm0oFKLl/GzoRykGjAYMRYwFAYDVQQDDA1KZXRQcm9maWxlIENBggkA0myxg7KDeeEwEwYDVR0lBAwwCgYIKwYBBQUHAwEwCwYDVR0PBAQDAgWgMA0GCSqGSIb3DQEBCwUAA4ICAQAF8uc+YJOHHwOFcPzmbjcxNDuGoOUIP+2h1R75Lecswb7ru2LWWSUMtXVKQzChLNPn/72W0k+oI056tgiwuG7M49LXp4zQVlQnFmWU1wwGvVhq5R63Rpjx1zjGUhcXgayu7+9zMUW596Lbomsg8qVve6euqsrFicYkIIuUu4zYPndJwfe0YkS5nY72SHnNdbPhEnN8wcB2Kz+OIG0lih3yz5EqFhld03bGp222ZQCIghCTVL6QBNadGsiN/lWLl4JdR3lJkZzlpFdiHijoVRdWeSWqM4y0t23c92HXKrgppoSV18XMxrWVdoSM3nuMHwxGhFyde05OdDtLpCv+jlWf5REAHHA201pAU6bJSZINyHDUTB+Beo28rRXSwSh3OUIvYwKNVeoBY+KwOJ7WnuTCUq1meE6GkKc4D/cXmgpOyW/1SmBz3XjVIi/zprZ0zf3qH5mkphtg6ksjKgKjmx1cXfZAAX6wcDBNaCL+Ortep1Dh8xDUbqbBVNBL4jbiL3i3xsfNiyJgaZ5sX7i8tmStEpLbPwvHcByuf59qJhV/bZOl8KqJBETCDJcY6O2aqhTUy+9x93ThKs1GKrRPePrWPluud7ttlgtRveit/pcBrnQcXOl1rHq7ByB8CFAxNotRUYL9IF5n3wJOgkPojMy6jetQA5Ogc8Sm7RG6vg1yow==
```

```
6ZUMD7WWWU-eyJsaWNlbnNlSWQiOiI2WlVNRDdXV1dVIiwibGljZW5zZWVOYW1lIjoiSmV0cyBHcm91cCIsImFzc2lnbmVlTmFtZSI6IiIsImFzc2lnbmVlRW1haWwiOiIiLCJsaWNlbnNlUmVzdHJpY3Rpb24iOiIiLCJjaGVja0NvbmN1cnJlbnRVc2UiOmZhbHNlLCJwcm9kdWN0cyI6W3siY29kZSI6IklJIiwiZmFsbGJhY2tEYXRlIjoiMjAxOS0wOS0wMyIsInBhaWRVcFRvIjoiMjAyMC0wOS0wMiJ9LHsiY29kZSI6IkFDIiwiZmFsbGJhY2tEYXRlIjoiMjAxOS0wOS0wMyIsInBhaWRVcFRvIjoiMjAyMC0wOS0wMiJ9LHsiY29kZSI6IkRQTiIsImZhbGxiYWNrRGF0ZSI6IjIwMTktMDktMDMiLCJwYWlkVXBUbyI6IjIwMjAtMDktMDIifSx7ImNvZGUiOiJQUyIsImZhbGxiYWNrRGF0ZSI6IjIwMTktMDktMDMiLCJwYWlkVXBUbyI6IjIwMjAtMDktMDIifSx7ImNvZGUiOiJHTyIsImZhbGxiYWNrRGF0ZSI6IjIwMTktMDktMDMiLCJwYWlkVXBUbyI6IjIwMjAtMDktMDIifSx7ImNvZGUiOiJETSIsImZhbGxiYWNrRGF0ZSI6IjIwMTktMDktMDMiLCJwYWlkVXBUbyI6IjIwMjAtMDktMDIifSx7ImNvZGUiOiJDTCIsImZhbGxiYWNrRGF0ZSI6IjIwMTktMDktMDMiLCJwYWlkVXBUbyI6IjIwMjAtMDktMDIifSx7ImNvZGUiOiJSUzAiLCJmYWxsYmFja0RhdGUiOiIyMDE5LTA5LTAzIiwicGFpZFVwVG8iOiIyMDIwLTA5LTAyIn0seyJjb2RlIjoiUkMiLCJmYWxsYmFja0RhdGUiOiIyMDE5LTA5LTAzIiwicGFpZFVwVG8iOiIyMDIwLTA5LTAyIn0seyJjb2RlIjoiUkQiLCJmYWxsYmFja0RhdGUiOiIyMDE5LTA5LTAzIiwicGFpZFVwVG8iOiIyMDIwLTA5LTAyIn0seyJjb2RlIjoiUEMiLCJmYWxsYmFja0RhdGUiOiIyMDE5LTA5LTAzIiwicGFpZFVwVG8iOiIyMDIwLTA5LTAyIn0seyJjb2RlIjoiUk0iLCJmYWxsYmFja0RhdGUiOiIyMDE5LTA5LTAzIiwicGFpZFVwVG8iOiIyMDIwLTA5LTAyIn0seyJjb2RlIjoiV1MiLCJmYWxsYmFja0RhdGUiOiIyMDE5LTA5LTAzIiwicGFpZFVwVG8iOiIyMDIwLTA5LTAyIn0seyJjb2RlIjoiREIiLCJmYWxsYmFja0RhdGUiOiIyMDE5LTA5LTAzIiwicGFpZFVwVG8iOiIyMDIwLTA5LTAyIn0seyJjb2RlIjoiREMiLCJmYWxsYmFja0RhdGUiOiIyMDE5LTA5LTAzIiwicGFpZFVwVG8iOiIyMDIwLTA5LTAyIn0seyJjb2RlIjoiUlNVIiwiZmFsbGJhY2tEYXRlIjoiMjAxOS0wOS0wMyIsInBhaWRVcFRvIjoiMjAyMC0wOS0wMiJ9XSwiaGFzaCI6IjE0Mjg5NzUwLzAiLCJncmFjZVBlcmlvZERheXMiOjcsImF1dG9Qcm9sb25nYXRlZCI6ZmFsc2UsImlzQXV0b1Byb2xvbmdhdGVkIjpmYWxzZX0=-Gd8RATyTEnHcAydKuC7N1ZdeLaMP9IR+nlPyVxvLsczAUTGKxcuAYbfz/uVtepg8ey4NfJlPNS+AGcGz8x7ImkX9jEV9KElMxPu3tKSdF/WKo6JCONX7UtudYa/9EQum3banxci/qH7jejSrFZSN+YjWQiYTR0Q8gq4/a2RyQTgseZfpImY/nXkOWLwWArr/p+4ddp/bWQN4nLTW+Z4ZaQeLE96Z9viCdn62EKOcR02Hfr9Oju9VYQh1L8pGrTqNey5nUSv/LQUbVwo5qoYbBRos8l6ewkFNGsuC3vtOgGWSgkgChbDjWhW4Nkm4vDM2NFAphMsS1dgyPw3eJ3C+6A==-MIIElTCCAn2gAwIBAgIBCTANBgkqhkiG9w0BAQsFADAYMRYwFAYDVQQDDA1KZXRQcm9maWxlIENBMB4XDTE4MTEwMTEyMjk0NloXDTIwMTEwMjEyMjk0NlowaDELMAkGA1UEBhMCQ1oxDjAMBgNVBAgMBU51c2xlMQ8wDQYDVQQHDAZQcmFndWUxGTAXBgNVBAoMEEpldEJyYWlucyBzLnIuby4xHTAbBgNVBAMMFHByb2QzeS1mcm9tLTIwMTgxMTAxMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAxcQkq+zdxlR2mmRYBPzGbUNdMN6OaXiXzxIWtMEkrJMO/5oUfQJbLLuMSMK0QHFmaI37WShyxZcfRCidwXjot4zmNBKnlyHodDij/78TmVqFl8nOeD5+07B8VEaIu7c3E1N+e1doC6wht4I4+IEmtsPAdoaj5WCQVQbrI8KeT8M9VcBIWX7fD0fhexfg3ZRt0xqwMcXGNp3DdJHiO0rCdU+Itv7EmtnSVq9jBG1usMSFvMowR25mju2JcPFp1+I4ZI+FqgR8gyG8oiNDyNEoAbsR3lOpI7grUYSvkB/xVy/VoklPCK2h0f0GJxFjnye8NT1PAywoyl7RmiAVRE/EKwIDAQABo4GZMIGWMAkGA1UdEwQCMAAwHQYDVR0OBBYEFGEpG9oZGcfLMGNBkY7SgHiMGgTcMEgGA1UdIwRBMD+AFKOetkhnQhI2Qb1t4Lm0oFKLl/GzoRykGjAYMRYwFAYDVQQDDA1KZXRQcm9maWxlIENBggkA0myxg7KDeeEwEwYDVR0lBAwwCgYIKwYBBQUHAwEwCwYDVR0PBAQDAgWgMA0GCSqGSIb3DQEBCwUAA4ICAQAF8uc+YJOHHwOFcPzmbjcxNDuGoOUIP+2h1R75Lecswb7ru2LWWSUMtXVKQzChLNPn/72W0k+oI056tgiwuG7M49LXp4zQVlQnFmWU1wwGvVhq5R63Rpjx1zjGUhcXgayu7+9zMUW596Lbomsg8qVve6euqsrFicYkIIuUu4zYPndJwfe0YkS5nY72SHnNdbPhEnN8wcB2Kz+OIG0lih3yz5EqFhld03bGp222ZQCIghCTVL6QBNadGsiN/lWLl4JdR3lJkZzlpFdiHijoVRdWeSWqM4y0t23c92HXKrgppoSV18XMxrWVdoSM3nuMHwxGhFyde05OdDtLpCv+jlWf5REAHHA201pAU6bJSZINyHDUTB+Beo28rRXSwSh3OUIvYwKNVeoBY+KwOJ7WnuTCUq1meE6GkKc4D/cXmgpOyW/1SmBz3XjVIi/zprZ0zf3qH5mkphtg6ksjKgKjmx1cXfZAAX6wcDBNaCL+Ortep1Dh8xDUbqbBVNBL4jbiL3i3xsfNiyJgaZ5sX7i8tmStEpLbPwvHcByuf59qJhV/bZOl8KqJBETCDJcY6O2aqhTUy+9x93ThKs1GKrRPePrWPluud7ttlgtRveit/pcBrnQcXOl1rHq7ByB8CFAxNotRUYL9IF5n3wJOgkPojMy6jetQA5Ogc8Sm7RG6vg1yow==
```

-->

### Idea 激活方法

#### Activetion Code

[在线生成](http://idea.iteblog.com/)

=======
<!--
各種泄露數據庫下載
RESILIO
下载数据库 BHMIILA2HRJ5ZG6FN6KE7YUKBZMQOFCOA
上传数据库 AMWD6B3LALQTZ34DJ7VWZS4PC3RJXJQER

ED2K下载链接
ed2k://|file|2010.06-江西移动全库-408万-access.7z|1329999527|5231E1EC5EE1123C6E694AD6399F9807|h=DORZC7XFNG63ZWX6C3RSN3Q7CWZXG5G4|/
ed2k://|file|2012.01-千脑-70万-csv.rar|34017079|A30DD3EF32C03C86E71032CDCA1C5EF9|h=2Z7TKJED7P2NJCKUCINNHMWLXV3KVVS4|/
ed2k://|file|2012.02-AcFun-15万-txt.rar|2241909|C2439FAB2BC7322273DE5D512A530A83|h=QJWQ3LWZ3UFJMPQHPD6WGXYYZHPRLQ43|/
ed2k://|file|2012.03-圆通数据库-mssql.rar|127496748|75F92807F541FB0EBB4773BA83D5157A|h=YAOCNQEUXCNBBTIM226NNZLJA7SMMSDS|/
ed2k://|file|2012.07-yahoo-45万-txt.bz2|6871089|8769EC2314C1AF2C98237DF58C7076D2|h=VSJ52KZ6O6JUZNZKXKT7F3LRXHBKJKMN|/
ed2k://|file|2012.08-小米论坛-828万-mysql.rar|518891223|87704FEA5B191C21F605A0C135BAF98E|h=6UQWS3OQ4VGUXLYW2L6H6TL2GKZOJAUA|/
ed2k://|file|2012.08-小米论坛-828万-txt.rar|361627120|2ED96D2F0E515321F67A31E84DC77B3C|h=UNNVFRMNWNP7UAIXZ6Y6AFCKOLBFJILW|/
ed2k://|file|2013.04-DNF-700万-mysql.zip|306178725|169CE4FA4D4F467BCB7F8297CE6EE032|h=C3KZ6C637ARBAPD5UNF2YMYMT5LTS2UK|/
ed2k://|file|2013.08-酒店开房记录-2000万-excel.rar|610164988|26F994CA1ABA72051ECE497F9AB7959A|h=EDLQDIHSRAJHB5SVNDQVMNPHOXVO3XB6|/
ed2k://|file|2013.08-酒店开房记录-2000万-mssql.bak|8030079488|6FCCDC6DE213DC72A4EFEE19AF2FC1AC|h=5YJSQJY46OYKYMQA5P4G3DUAQGATYDFI|/
ed2k://|file|2014.08-企业400号段数据-mssql.rar|46506453|4F44726413F3B9F9F701635FB498EAAB|h=LP47JMAJGOX233HQR2V3K673G7LE22RI|/
ed2k://|file|2014.08-台湾某财经电视台数据库-2014-txt.zip|53519|95160AAE4A9E3074BACB04C606C0748F|h=3KQJJ4ADWKNOGNJIZIICBXQ5SLPD62R5|/
ed2k://|file|2014.08-房产网-11万-sql.7z|6095432|D99DE175A27D179A5EB9F34D2D975FB0|h=2GN2RLDSDDVZ4POQZVIEJODQJVH2CJ4G|/
ed2k://|file|2014.09-mail.ru邮箱地址-466万-txt.7z|30715779|5247DC686608FD2317A31E8BA67899F4|h=DFVLYBFEQQLDZSXIEOWHWY2BMA5DKDBO|/
ed2k://|file|2014.09-yandex.ru-100万-txt.zip|16200283|80C4A344D51DBAE12F0A0D50202E9313|h=RA2KA6RRGELDAMXBAKXVFI3W7SIJ6TEE|/
ed2k://|file|2014.12-12306-13万-txt.7z|4470710|7B25F299C7862BFA855B63B04BB00E2A|h=VURCVAXE4UVFI2TOIEC6DIZUBSYELY76|/
ed2k://|file|2016.04-卡塔尔国家银行QNB-csv.zip|534384790|D7D81061307568AE47A3EE6C894D6C6C|h=VRQGQASTAHXFRGBZXAAIABVTFJRRIV7G|/
ed2k://|file|2016.04-土耳其公民数据mernis-5000万-sql.gz|1555520122|22B660CB494D89FC84198A6EEA66E3B6|h=HYBIW22P3G56CUB7RR34CJVD7RKO34BS|/
ed2k://|file|2011.03-多玩游戏网-800万-txt.rar|227441723|F8388A178222518978550D3E64B6129B|h=XMR2CYVQI3HOMKVRGUCCFGYZ3JVHKLCG|/
ed2k://|file|2011.03-当当网买家信息-101万-Excel.zip|7822098|1F66086AE57B74D69BF75A2EF7900B2E|h=VRWZME24KH7UTIF3HPTCO5V5KNTEHUAQ|/
ed2k://|file|2011.04-766游戏网-12万-sql.rar|5031951|BBE2D87564A2A8E4B083B57C697FD24E|h=DUFDLSY2A4F5SPZMMCN5JP7TE2HWA4EV|/
ed2k://|file|2011.04-IS语音-969万-txt.zip|177030850|B153DDF9FE16EFFF30C589664592F85A|h=HCB5NVNHVGVGKMDCS7HXHI4MNQASG5SY|/
ed2k://|file|2011.04-亚马逊中国买家信息-20万.zip|7570413|356D9E9C07D62243EF8A62745819E85C|h=BXLWB7OFKIFTCSCUU4Y47DHMX67GF7DO|/
ed2k://|file|2011.04-凡客诚品买家信息-20万-Excel.zip|7784030|AEC527EA7E816DBD75FF92B0C26BC480|h=VXC2RO23H23OCZISUXTEO62RTVHGQFPZ|/
ed2k://|file|2011.04-爱拍游戏网-1100万-txt.zip|267845795|87F9FFE887B0F53CAFD2A11205CB6C52|h=G6AQRSNJ7CHDTX5MTV6RYGB2OHYOAEXA|/
ed2k://|file|2011.05-木蚂蚁-13万-sql.zip|8598547|680F8999D4E27174553D1C11118DF978|h=5G2YZ7Z6RAQ5M5XUNCEFNX7ZYAITMZPZ|/
ed2k://|file|2011.07-土木在线-540万-sql.zip|645903048|4ED3B64224752DE3AB11B11D2FD9DA06|h=UL3F74NI266IR4IHI7UHDKMZRQMX3PFX|/
ed2k://|file|2011.10-178游戏网-1000万-txt.rar|108534783|FFCD04A52339701C8CB5197BDCF9F4DC|h=C2UYTR264YXVM6NSJNUV5R2PC5VZNAYU|/
ed2k://|file|2011.10-CSDN.NET-600万-sql.rar|109942505|A29D9468556CF73AFB48A3A8427629DC|h=VTPXT56G3BGRTHBROKQEWW6XAQTMYPLZ|/
ed2k://|file|2011.10-嘟嘟牛-66277-txt.rar|215666725|EF7187E33A8EBD9FD806343B7B1CAA82|h=Z5YU2Z6P6GUT5DUKQ6L4X5YFMZZNZ4YZ|/
ed2k://|file|2011.11-7k7k小游戏-2000万-txt.rar|203648704|6EB70910C1C193F5BE04610B503EF4A0|h=Y4ITT7C5Z5LOOREJPWXA25TM2NLKEEDX|/
ed2k://|file|2011.11-人人网-500万-txt.rar|51969611|8CD19B7A2EB9F1F74CB8BFBDE7BD144D|h=SDNOOZCYR6PXZIRZTZPEICNRNZ67BQJJ|/
ed2k://|file|2011.12-天涯社区-4000万-txt.rar|493480455|E4E0CFD85E2A783A3C3BD2539AA28FC3|h=4FB7J7QPRWRIPX7QWWTYVZCKMWDZ5VIQ|/
ed2k://|file|2011.12-淘宝买家卖家邮箱-2500万-txt.zip|135534861|F40C3C9F32F2C30B1A2484FAB3CB1257|h=GLUDUAAYPAALG3GPHD4EHT5OB6V6WBVB|/
ed2k://|file|2012.10-QQ精准客户名单-4500万-txt.rar|131416815|134F81AA90B27F55818E7A521D3CB35B|h=NRF2HAH2IXDT635UV6NDEGSA2HSOSSHZ|/
ed2k://|file|2012.06-LinkedIn-16737万-txt.rar|7503170474|A50C488915FC70E1DE644AA5F3432D6F|h=E2NEXLXOOA6PONPKUGVRVIMEU54EC6P4|/
ed2k://|file|2013.06-Myspace.com-36021万-txt.7z|12419587039|A1B14F88891885D636DE9F642A3E06DF|h=3QBXWEHRBUSUEWJOSHCF47B7HEC4Q5BM|/
-->

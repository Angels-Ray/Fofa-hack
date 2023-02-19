# Fofa-hack

### 简介

基于[fofa_spider-1.0.5](https://github.com/FightingForWhat/fofa_spider-1.0.5) - 非付费会员，fofa数据无限抓取版 的梅开二度，配置普通用户账号密码即可使用

截止至 `2023-2-16` 日 ，亲测可用，如果项目不行了欢迎联系我

### 使用

```shell
git clone https://github.com/Cl0udG0d/Fofa-hack
```

安装运行所需的库文件，国内请加源 https://pypi.tuna.tsinghua.edu.cn/simple

```shell
pip install -r requirements.txt
```

配置`config.py`中的`fofa_account`，支持多账号
```json
fofa_account=[
    {
        "fofa_username" : "test@email.com",
        "fofa_password" : "12345678"
    },
  {
        "fofa_username" : "test1@email.com",
        "fofa_password" : "12345678"
    }
]
```

也就是你的FOFA账号密码

> 因为有朋友说ddddocr这个库在不同版本的操作系统上会有各种运行的错误,为了避免完全用不了Fofa-hack
> 
> 现在将老版本的方式重新给出,如果账号密码登录不了,或者单纯不想用账号密码登录的时候,可以直接复制cookie登录

[ddddocr出现问题跳转此处查看](docs/QUESTIONS.md#ddddocr错误解决)

运行`fofa.py`

> python3 fofa.py

爬取的结果会存储到`md5(搜索关键字)_运行时间戳.txt`文件中

### 参数
<details>
<summary>config参数详情</summary>
<table >
  <tr>
    <td>参数值</td>
    <td>释义</td>
  </tr>
  <tr>
    <td>VERSION_NUM</td>
    <td>Fofa-hack 版本号</td>
  </tr>
<tr>
    <td>MAX_LOGIN_RETRY_NUM</td>
    <td>登录最大重试次数</td>
  </tr>
<tr>
    <td>MAX_MATCH_RETRY_NUM</td>
    <td>页面URL获取最大重试次数</td>
  </tr>
</table>
</details>

### 测试

输入 搜索关键字 `app="ThinkPHP"`，等待秒数为5的情况下，下载1-50页数据经过测试无问题，经过自动去重之后剩余497条

### 使用问题集合

详情请见[QUESTIONS](docs/QUESTIONS.md)

### 更新日志

详情请见[CHANGELOG](docs/CHANGELOG.md)

### TODO List
<details>
<summary>TODO</summary>
<table >
  <tr>
    <td>名称</td>
    <td>简介</td>
  </tr>
  <tr>
    <td>支持输入参数</td>
    <td>支持 --proxy这种输入参数的形式运行脚本</td>
  </tr>
<tr>
    <td>支持代理池</td>
    <td>使用代理池的方式防止FOFA断开连接</td>
  </tr>
<tr>
    <td>支持多种导出格式</td>
    <td>支持json、txt、excel等方式导出结果</td>
  </tr>
<tr>
    <td>支持多种爬取内容</td>
    <td>添加支持title、status、headers等内容</td>
  </tr>
<tr>
    <td>增加程序稳定性</td>
    <td>防止程序因为各种情况运行失败或者被ban的情况</td>
  </tr>
</table>
</details>

### 贡献者

<!-- readme: collaborators,contributors -start -->
<table>
<tr>
    <td align="center">
        <a href="https://github.com/Cl0udG0d">
            <img src="https://avatars.githubusercontent.com/u/45556496?v=4" width="100;" alt="Cl0udG0d"/>
            <br />
            <sub><b>潘一二三</b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/wanswu">
            <img src="https://avatars.githubusercontent.com/u/49047734?v=4" width="100;" alt="wanswu"/>
            <br />
            <sub><b>Wans</b></sub>
        </a>
    </td></tr>
</table>
<!-- readme: collaborators,contributors -end -->

### END 

网络乞丐在线乞讨
<div>
    <img  alt="PNG" src="./images/sponsor.png"  width="280px" />
</div>

建了一个微信的安全交流群，欢迎添加我微信备注`进群`，一起来聊天吹水哇，以及一个会发布安全相关内容的公众号，欢迎关注 :)

<div>
    <img  alt="GIF" src="https://springbird.oss-cn-beijing.aliyuncs.com/img/mmqrcode1632325540724.png"  width="280px" />
    <img  alt="GIF" src="https://springbird.oss-cn-beijing.aliyuncs.com/img/qrcode_for_gh_cead8e1080d6_344.jpg"  width="280px" />
</div>

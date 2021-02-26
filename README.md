# 合成大西瓜(スイカゲーム)

**このプロジェクトはテクノロジーとエンターテインメントの学習にのみ役立つことを宣言します。侵害を避けるために、変更されたWebサイトを大規模に広めたり商品化したりしないでください！**

> 最も単純なアプリのリリースは『 合成大西瓜 』，ダイアグラム変更ツールをサポートし、コードを変更する必要はありません。構成を変更するだけです。
>
> ご不明な点がございましたら、こちらまでお問い合わせください。：liyupi66
> 
> 著者プログラミング技術公開番号[『 程序员鱼皮 』](https://mp.weixin.qq.com/s/H9VR1MWn-9bKSC_1l_MkJw)，ファローぜひ ❤️
>
> 問題が発生した場合は、最初にこのドキュメントを読んでください[ 问题及解决 ](#问题及解决)

細かい説明の入ったチュートリアル：[魔改和上线你的合成大西瓜，最全教程！](https://mp.weixin.qq.com/s/H9VR1MWn-9bKSC_1l_MkJw)

動画のチュートリアル：[全网最贴心的魔改合成大西瓜教程，从修改到发布！](https://www.bilibili.com/video/BV1Vy4y1n7KW/)

オンラインで再生するための変更されていないバージョン：[https://daxigua.liyupi.com](https://daxigua.liyupi.com)

オンラインでプレイするためのバージョン：[https://dadaxigua.liyupi.com](https://dadaxigua.liyupi.com)

変更されていないソースコード：[https://github.com/liyupi/daxigua/releases/tag/1.0.0](https://github.com/liyupi/daxigua/releases/tag/1.0.0)

🔥 [大型スイカのリマップツールを新発売、リマップ効率が2倍に！](https://daxigua-tools.liyupi.com)

![秀爆朋友圈](./assets/dadaxigua.png)

### 目次

- [ローカルで開始](#ローカルで開始)

- [一瞬で終わらせる](#一瞬で終わらせる)

- [オンラインリリース](#オンラインリリース)

- [魔改原理](#魔改原理)

- [問題と解決策](#問題と解決策)


### ローカルで開始

> 2つのローカル起動方法があります。serveとDockerが提供されています。Xiaobaiは最初の方法をお勧めします。

#### 初心者用

1. serveをインストール：

    ```bash
    npm i -g serve
    ```

2. daxiguaディレクトリに入り、serveを実行：

    ```bash
    serve
    ```
   
3. ブラウザを開いてlocalhost:5000にアクセスするだけでOK!

#### Dockerはインストールされています。

> ありがとう [buchenglei](https://github.com/buchenglei) 

1. ボルド方法
    
    ```bash
    docker build -t daxigua-server .
    ```

2. サービスを実行させます

    ```bash
    docker run -d --name play-daxigua -p5000:5000 daxigua-server
    ```

### 一瞬で終わらせる

> 以下の指示に従って修正し、追加を続けるだけです。

1. スコアを変更する：extraSettings.jsファイルを変更する

2.画像を変更する：画像の指定されたディレクトリのres/raw-assetsディレクトリを置き換えるには、同じファイル名、接尾辞、サイズ、成功したオーバーライドを有効にすることができます、[材料文書を置き換えることができます](https://docs.qq.com/sheet/DS0d2VVVJYmpvZ0pZ)

3.無敵モード：extraSettings.jsファイルを変更する

4.最初のフルーツを指定する：extraSettings.jsファイルを変更する

5. 次のフルーツを指定する: extraSettings.jsファイルを変更する

6.大きな果実を小さな果実に：extraSettings.jsファイルを変更する

7.果実をよりQチップにする：extraSettings.jsファイルを変更し、[schema reference](https://docs.cocos.com/creator/api/zh/classes/PhysicsCircleCollider.html?h=circlecollider) )

8. 果物の落下を遅らせる: extraSettings.jsファイルの変更、[schema reference](https://docs.cocos.com/creator/manual/zh/physics/physics/rigid-body.html?h=%E5%88%9A%E4%) BD%93)

9. 音楽を置き換える: res/raw-assetsディレクトリ内の同じ音楽を上書きする、[置換可能な素材ファイル](https://docs.qq.com/sheet/DS0d2VVVJYmpvZ0pZ)

10.背景を置き換える:イメージの原則を変更することは同じですが、[材料文書を置き換えることができます](https://docs.qq.com/sheet/DS0d2VVVJYmpvZ0pZ)

11.広告を削除：広告画像を[同じ背景色の背景画像]に置き換える(https://636f-codenav-8grj8px727565176-1256524210.tcb.qcloud.la/0.png)

12. 広告リンクを置き換える: extraSettings.jsファイルを変更する

13. サイトタイトルの変更: extraSettings.jsファイルの変更

14. select pointsポップアップを開く: extraSettings.jsファイルを変更します。

15.右上のアイコンをクリックしてフルーツを変更する：変更 extraSettings.js

www.DeepL.com/Translator（無料版）で翻訳しました。


### オンラインリリース

> 提供了多种上线发布方式，腾讯云一键部署、Vercel、腾讯云静态网站托管、GitHub Pages 等，小白建议使用 Vercel。

>オンライン公開の方法は、Tencent Cloud ワンクリックデプロイ、Vercel、Tencent Cloud 静的ウェブホスティング、GitHub Pagesなどがあり、白人の方にはVercelがお勧めです。

#### テンセントクラウドワンクリック展開

リポジトリをフォークしてコードを投稿できる学生向け

下のボタンをクリックすると、何もせずに私のリポジトリをTencent Cloudにデプロイすることができます ⬇️。

> 自分のリポジトリをワンクリックでデプロイしたい場合は、まず自分のリポジトリをフォークして、ローカルで修正してからフォークリポジトリに投稿し、最後にワンクリックでデプロイボタンのリポジトリアドレスを自分のリポジトリに変更する必要があります!


#### ヴェルセル

運用が簡単でドメインも短いが、海外サーバーなため遅い

Vercelは無料のウェブホスティングプラットフォームで、ウェブサイトの展開やアクセス可能な短いURLの生成、購入したドメインへのバインド機能を提供してくれます。

コマンドラインから npm コマンドで Vercel をインストールします。

```
npm install -g vercel
```

インストールしたら、`index.html`ディレクトリ(私のはdaxigua)に移動し、`vercel`コマンドを使ってサイトを公開する。

```
cd daxigua
vercel --prod
```

次に、プロジェクト名、既存のプロジェクトと関連付けるかどうか、現在の設定を保存するかどうかなど、いくつかのオプションを入力するように求められます。 複数のプロジェクトを作成する場合は、既存のプロジェクトと関連付けないようにしましょう

無事に公開すると、URLが出てきて、それを開いてゲームを見ることができ、URLを共有することができます。



#### 腾讯云静态网站托管

中国サーバーです。リンクもmicrosoftにブロックされない。

住所： https://cloud.tencent.com/product/wh

この記事を参考にして掲載してみてください[マジックチェンジとオンラインであなたの合成大スイカ、完全版チュートリアル！](https://mp.weixin.qq.com/s/H9VR1MWn-9bKSC_1l_MkJw)



### 魔改原理
最初にお読みください：[魔法改造で合成大スイカをオンラインにする！チュートリアル完全版](https://mp.weixin.qq.com/s/H9VR1MWn-9bKSC_1l_MkJw)

project.js`ファイルにコメントを追加したので、「チェンジスコア」などのキーワードで検索するとすぐに見つけられ、修正の原理を学ぶことができます。

### 问题及解决

1. 无法安装 serve 或者 Vercel？

    答：如果报找不到 npm，请先安装 npm。

    如果安装中卡住，试着按下键盘（可能假死），还不行的话先用 npm 安装 cnpm（国内镜像，比较快）：
    
    ```bash
    npm install cnpm -g --registry=https://registry.npm.taobao.org 
    ```
    
    再用 cnpm 安装： `cnpm i -g serve` 或 `cnpm i -g vercel`
    
2. Vercel 网址被微信拦截怎么办？
   
    答：可以把网址复制到浏览器打开，也可以申请一个域名，在 Vercel 和服务提供商配置域名解析。
    Vercel 基本是海外的服务器，无需备案。

3. 怎么在电脑上浏览网页游戏？
   
    答：在浏览器中，按 F12 打开开发者工具，点击像手机一样的图标即可。
    
4. 为什么 serve 后，打开网页一片空白？

    答：大概率是你在错误的目录下执行了 serve，请务必在 index.html 所在的文件夹下执行 serve。

5. 执行 vercel 命令显示 signUp？

    答：要先去 [Vercel 官网](https://vercel.com/) 注册。

6. vercel 邮箱验证失败？

    答：先确认邮箱是否正确，如果验证失败，大概率是网络原因，请尝试 4G 等网络。或者在其他浏览器中，打开邮箱，点击验证按钮。

7. 怎么使用 vercel 同时上线多个版本？

    答：在输入 vercel 后，选择不和已有项目关联（link），并且使用一个新的项目名（project name）。

8. 想在修改文件后重新搞个新版本，但输入 vercel prod 后，直接覆盖了，而没有让我选择是否和现有项目关联（link），怎么办？
    
    答：执行 vercel 后，会在本地生成 `.vercel` 隐藏目录保存之前的发布信息，删掉该目录即可。

9. 导出网址后，我修改了图片，然后游戏中还是原来的图片？
    
    答：网址读取的是远程的文件，只改了本地当然没用！再次执行 vercel 或腾讯云命令，把最新文件传上去。
    
10. Mac 能否使用这个教程呢？
    
    答：当然可以！所有命令和 windows 完全一致！只是 cmd 命令行工具改为用 terminal 终端（按 command + 空格，搜索 terminal）
 
11. 为什么打开网站白屏了？
    
    答：大概率是你修改错误，导致一些文件缺失。。可以试试重新下载代码，再修改，请先确保本地可以运行，再发布！

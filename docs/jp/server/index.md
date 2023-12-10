# サーバーを構築する
このガイドでは、HomuraMCを利用してMinecraftサーバーを構築する事ができます。
## システム要件
### 対応バージョン
| Minecraft Version |  |
| ---- | ---- |
| ~1.16.3 | × |
| 1.16.4 / 1.16.5 | ◯ |
| 1.17~ | × |
| 統合版 | × |

段階的に全てのバージョンに対応する予定です。

### 対応OS
| OS |  |
| ---- | ---- |
| Windows | △<a href="#sys-ok-1"><small>*1</small></a> |
| Mac | △<a href="#sys-ok-2"><small>*1</small></a> |
| Linux | ◯ |

<a id="sys-ok-1"></a><small>*1 WSLを使用することで動かすことができます。なのでWindows 10 / Windows 11でしか動作しません。</small><br>
<a id="sys-ok-2"></a><small>*2 動作を確認できていない</small>

### 必須スペック
| スペック |  |
| ---- | ---- |
| CPU | 1GHz |
| RAM | 2GB |
| 記憶デバイス | 512MB |

### 推奨スペック
| スペック |  |
| ---- | ---- |
| CPU | 2.5GHz |
| RAM | 4GB |
| 記憶デバイス | 1024MB |

## サーバーの構築
### Pythonのインストール
Windowsの場合は[こちら](https://www.python.org/downloads/windows/)から、  
Macの場合は[こちら](https://www.python.org/downloads/macos/)から、  
Ubuntuの場合は[こちら](https://www.python.jp/install/ubuntu/index.html)から、  
それ以外のLinuxの場合は[こちら](https://www.python.jp/install/centos/index.html)  
から、Pythonをダウンロードしてインストールします。  
インストールできた場合は、次のステップに進みましょう。

### Gitのインストール
[こちら](https://git-scm.com/downloads)から、Gitをダウンロードしてインストールします。  
インストールできた場合は、次のステップに進みましょう。

### HomuraMCの環境構築・ビルド
まず、このコマンドを好きなフォルダで実行します。
```
git clone https://github.com/HomuraMC/Homura.git
```
次に、Pythonの仮想環境を作成します。(推奨)
```
python3 -m venv homura
```
仮想環境を作成した場合は、次のコマンドを使用して仮想環境にPythonにアクセスしてください。
```
cd ./homura/scripts/Activate
```
次に、pipを使用して、Homuraが必要とするライブラリをインストールします。  
```
python3 -m pip install -r requirements.txt
```
インストール後、次のコマンドを実行してサーバーを開始できます。  
```
python3 main.py
```
おめでとうございます！ここまでエラーも出ずにできた場合は、HomuraMCのビルドに成功しました！  
  
<div style="display: flex;">
	<div class="maeato">
		<b>前</b><br>
		<a href="/docs/jp/">メインページ</a>
	</div>

	<div class="maeato">
		<b>次</b><br>
		<a href="/docs/jp/config">コンフィグ</a>
	</div>
</div>
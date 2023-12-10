---
layout: jp
title: コンフィグ
lang: ja-JP
---
# コンフィグ
HomuraMCのHomura.iniファイルは、HomuraMCの設定を変更するためのファイルです。
<div class="alert alert-warning" role="alert">
	<b>Warning</b><br>
	このHomura.iniファイルは、config.ymlに置き換え予定です。
</div>

## EURAへの同意
初回起動時に「You do not agree with the eula! The eula can be read at https://aka.ms/MinecraftEULA and to agree, set the eula to True in Homura.ini.」というエラーが出たら、[MinecraftのEURA](https://aka.ms/MinecraftEULA)を読んで、Homura.ini内の```eula = False```を```eula = True```にしましょう。

## 説明
<table class="table table-striped">
	<tr>
		<td>Key</td>
		<td>Default value</td>
		<td>説明</td>
	</tr>
	<tr>
		<td>config_version</td>
		<td>1</td>
		<td>バージョンアップでコンフィグファイルが変更されたときに+1されます。</td>
	</tr>
	<tr>
		<td>server_ip</td>
		<td>0.0.0.0</td>
		<td>これは常に0.0.0.0のままなはずです。</td>
	</tr>
	<tr>
		<td>port</td>
		<td>25565</td>
		<td>サーバーをリッスンするポート。</td>
	</tr>
	<tr>
		<td>motd</td>
		<td>A Minecraft Server</td>
		<td>Minecraftのマルチプレイ画面に表示される説明。</td>
	</tr>
	<tr>
		<td>max_players</td>
		<td>20</td>
		<td>プレイヤーが接続できる最大の数。</td>
	</tr>
	<tr>
		<td>server_icon</td>
		<td>server_icon_path_here</td>
		<td>サーバーアイコンのパス。</td>
	</tr>
	<tr>
		<td>eula</td>
		<td>False</td>
		<td>MinecraftのEURAに同意したかどうか。</td>
	</tr>
</table>

```
[HomuraMC]
config_version = 1
server_ip = 0.0.0.0
port = 25565
motd = A Minecraft Server
max_players = 20
server_icon = server_icon_path_here
eula = False
```

<div style="display: flex;">
	<div class="maeato">
		<b>前</b><br>
		<a href="/docs/jp/server/">サーバーを構築する</a>
	</div>

	<div class="maeato">
		<b>次</b><br>
		<a href="/docs/jp/plugin/">プラグインを書く</a>
	</div>
</div>
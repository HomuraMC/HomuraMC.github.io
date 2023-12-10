# コンフィグ
HomuraMCのHomura.iniファイルは、HomuraMCの設定を変更するためのファイルです。
<div class="alert alert-warning" role="alert">
	<b>Warning</b><br>
	このHomura.iniファイルは、config.ymlに置き換え予定です。
</div>

## EURAへの同意
初回起動時に「You do not agree with the eula! The eula can be read at https://aka.ms/MinecraftEULA and to agree, set the eula to True in Homura.ini.」というエラーが出たら、[MinecraftのEURA](https://aka.ms/MinecraftEULA)を読んで、Homura.ini内の```eula = False```を```eula = True```にしましょう。

## 説明
| Key | Default value | 説明 |
| ---- | ---- | ---- |
| config_version | 1 | バージョンアップでコンフィグファイルが変更されたときに+1されます。 |
| server_ip | 0.0.0.0 | これは常に0.0.0.0のままなはずです。 |
| port | 25565 | サーバーをリッスンするポート。 |
| motd | A Minecraft Server | Minecraftのマルチプレイ画面に表示される説明。 |
| max_players | 20 | プレイヤーが接続できる最大の数。 |
| server_icon | server_icon_path_here | サーバーアイコンのパス。 |
| eula | False | MinecraftのEURAに同意したかどうか。 |

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
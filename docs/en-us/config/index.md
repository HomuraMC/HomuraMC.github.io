---
layout: default
title: Config
lang: en-US
---
# Config
The Homura.ini file of HomuraMC is used to change the settings of HomuraMC.
<div class="alert alert-warning" role="alert">
	<b>Warning</b><br>
	This Homura.ini file will be replaced by config.yml.
</div>

## Agreement to EURA
If you get the error "You do not agree with the eula! The eula can be read at https://aka.ms/MinecraftEULA and to agree, set the eula to True in Homura.ini." on first startup, Read [EURA in Minecraft](https://aka.ms/MinecraftEULA) and set ``eula = False`` to ``eula = True`` in Homura.ini.

## Description
<table class="table table table-striped">
	<tr>
		<td>Key</td>
		<td>Default value</td>
		<td>Description</td>
	</tr>
	<tr>
		<td>config_version</td>
		<td>1</td>
		<td>It is +1 when the config file is changed by version up.</td>
	</tr>
	<tr>
		<td>server_ip</td>
		<td>0.0.0.0</td>
		<td>This should always remain 0.0.0.0. </td>
	</tr>
	<tr>
		<td>port</td>
		<td>25565</td>
		<td>Port to listen for servers. </td>
	</tr>
	<tr>
		<td>motd</td>
		<td>A Minecraft Server</td>.
		<td>A description that appears on the Minecraft multiplayer screen. </td>
	</tr>
	<tr>
		<td>max_players</td>
		<td>20</td>
		<td>Maximum number of connections a player can make. </td>
	</tr>
	<tr>
		<td>server_icon</td>
		<td>server_icon_path_here</td>
		<td>Path of the server icon. </td>
	</tr>
	<tr>
		<td>eula</td>
		<td>False</td>
		<td>Whether you agree with Minecraft's EURA. </td>
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
		<b>back</b><br>
		<a href="/docs/jp/server/">Build a server</a>
	</div>

	<div class="maeato">
		<b>next</b><br>
		<a href="/docs/jp/plugin/">Writing Plugins</a>
	</div>
</div>
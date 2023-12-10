---layout: default
layout: default
title: write plugin
lang: en-US
--- layout: default
# write plugin
In this guide, you can use HomuraMC's Plugin API to create mini-games and many other things.  
## Plugin template
{% highlight python %}
from classes import HomuraServerProtocol

class HomuraMCPluginBackends():
	@staticmethod
	def getPluginName():
		return "MyCoolPlugin"
	@staticmethod
	def getPluginDescription():
		return "MyCoolPlugin by nennneko5787"
	@staticmethod
	def getPluginAuthors():
		return ["nennneko5787"]
	@staticmethod
	def getPluginVersion():
		return "0.0.1"

class HomuraMCPlugin():
	@staticmethod
	def onLoad():
		print("Loaded")
	@staticmethod
	def onJoinPlayer(self):
		self.factory.send_msg(f"[Server] Hello!", self.display_name)
		return f"{self.display_name} joined"
	@staticmethod
	def onQuitPlayer(self):
		return f"{self.display_name} leaved"
	@staticmethod
	def onChat(self,p_text):
		if p_text == "hello":
			self.send_packet('title',
					self.buff_type.pack_varint(0),
					self.buff_type.pack_chat(f"§aHello {self.display_name}"),
				)
{% endhighlight %}
In this way, plugins can be written.
<div style="display: flex;">
	<div class="maeato">
		<b>back</b><br>
		<a href="/docs/en-us/config/">Config</a>
	</div>
</div>
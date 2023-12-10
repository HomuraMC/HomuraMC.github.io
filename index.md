---
layout: default
title: Main Page
lang: en
---
# HomuraMC
a Minecraft server software
## Gallery
{% highlight python %}
from classes import HomuraServerProtocol

class HomuraMCPlugin():
	@staticmethod
	def onChat(self,p_text):
		if p_text == "hello":
			self.send_packet('title',
					self.buff_type.pack_varint(0),
					self.buff_type.pack_chat(f"§aHello {self.display_name}"),
				)
{% endhighlight %}
<a href="./screenshots/2023-12-10_11.23.12.png" data-lightbox="group"><img src="./screenshots/2023-12-10_11.23.12.png" class="resize"></a>
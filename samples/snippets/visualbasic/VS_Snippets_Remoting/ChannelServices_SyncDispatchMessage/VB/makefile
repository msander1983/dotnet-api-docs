all: Share.dll server.exe client.exe

Share.dll: ChannelServices_syncdispatchmessage_Share.vb
	vbc /t:library ChannelServices_syncdispatchmessage_Share.vb

server.exe: ChannelServices_syncdispatchmessage_Server.vb ChannelServices_syncdispatchmessage_Share.dll
	vbc ChannelServices_syncdispatchmessage_Server.vb /r:ChannelServices_syncdispatchmessage_Share.dll

client.exe: channelservices_syncdispatchmessage_client.vb ChannelServices_syncdispatchmessage_Share.dll
	vbc ChannelServices_syncdispatchmessage_client.vb /r:ChannelServices_syncdispatchmessage_Share.dll
# tungsten

Protect your server from cheaters, quickly.

Tungsten is a performance fork of orebfuscator, aimed to optimise it for large servers and custom maps alike. This is a work in progress, with only one stable version built. Updates will be pushed here, so keep yourself informed.

# How it works:

It works like orebfuscator, by obfuscating blocks that arent in the players view, so they cannot request blocks out of their view. 

For Example:

Player X is in a solid box made of grass, with no way to look out. Usually, if the player uses xRay to detect a block (e.g andesite) under itself out of its FOV, the server would tell the client the location of andesite.

Now, with Tungsten installed:

Same circumstances.
Player xRays - he sees random blocks spammed everywhere because the blocks under the box are blocks he cannot see. His xRays do not pass through blocks, therefore not letting him see through blocks.

# About
I was looking for a anti xRay plugin like orebfuscator, but for smaller and less performant servers. Sadly, noone really made a fork of orebfuscator. I also tested on a discrete server, by modrinth hosting. It also seems to have some trouble with custom maps, deployed by many earth servers. Thats why I forked orebfuscator and released this. I named it tungsten because tungsten reflects radiation/xRays/neutrons back to the source, it is also what killed Harry Daghlian during his demon core experiment. (Read more: https://www.lindahall.org/about/news/scientist-of-the-day/harry-daghlian/ )

# Installation: 

Everything you need is in the repository. You will need ProtocolLib.

If you're using a GUI based system, drag the plugin and its dependency, ProtocolLib, into your plugins folder.

If you're using CLI, use 

mv /your/path/to/plugin/tungsten-plugin--b1.jar /your/path/to/plugins && mv /your/path/to/plugin/ProtocolLib.jar /your/path/to/plugins

Replace your/path/to to the path of both jar files.

If you have issues, feel free to contact me via GitHub Issues

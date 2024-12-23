# TheHunter: call of the wild settings files
Settings files from TheHunter: Call of the wild as XMLs

##Introduction
Settings files in Avalanche Studios titles are responsible for fundamental functions, like listing spawnable entities and having basic settings for a bunch of things
However, they come as .bin files, a custom format you can't just edit like a text file and unlike Just Cause 3 and 4, TheHunter COTW has no tool to unpack them to xml, which would let you easily edit them without a hex editor or other tools

##So what is this?

Even though TheHunter COTW is quite similar to Just Cause 3, its settings files are different enough to throw off the Just Cause 3 tools and prevent them form unpacking them. Just Cause 3's tools work on a number of other TheHunter COTW files, so I thought to myself "the settings files can't be too different" and wondered what would happen if I re-created them the way they would look in Just Cause 3, repacked them with Just Cause 3's tools and loaded them into TheHunter COTW

And...it works! Seems TheHunter COTW is backwards compatible with Just Cause 3's bin format. I'm mainly using the output [Deca](https://github.com/kk49/deca) produces to fully re-create them from srcratch. This is still a WIP, but the goal is to re-create all proper bin files as xml

##What do you mean by "proper bin files"

Proper bin files are RTPCs, the same file type entity, location and minigame configuration files use (epe, nl/fl, blo)
However Avalanche is moving towards using ADF for more and more things. ADF was originally mainly used for stat-files in Just Cause 3, but is increasingly used in other areas as well such as models and additional configuration files. They seem to be more versatile and performant than RTPC

Some bin files in TheHunter COTW are already actually ADF files, which I'm pretty sure I can not re-create in this way, so I am only remaking the RTPC bin files

##Ok but how can I use these files?
Simply download all the XMLs. Also get the most recent [Just Cause 3 tools package](https://drive.google.com/file/d/13Iijzxg2wUUh9w-OqzomlaN5XGixLp7x/view?usp=drive_link) and extract it

Edit the settings file you want, save it and drag the xml onto JustCause3_Batch.bat and it will repack the xml back to a bin file
Now just add your edited file to your dropzone folder at the same path they are here and enjoy!

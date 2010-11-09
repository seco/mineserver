Mineserver
==========
by Fador & Psoden

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

Custom Minecraft Alpha server software written in C++.

NOTICE
------
Currently in development. (Alpha stage)
Server still lacks some critical features
and should be only used for testing.

Tested to build on Windows (Visual Studio 2010 project included) and on Linux (Makefile included).

We are trying to minimize memory and cpu usage compared to original Java server.

Features
--------
 * some chat commands, more to come..
 * own NBT parsing/saving
 * Lightmap generation
 * Config file
  
ToDo (Arranged by priority)
---------------------------
 * Item pickup
 * Map generation
 * Physics
 * Growing trees etc.
 * and more
 
Chat commands
-------------

**For all players**

*  /players : Lists online players
*  /about : Server name & version
*  /rules : Shows server rules

**Admin only**

*  %<text> : Servermessage 
*  &<text> : Admin-only message
*  /kick <nick> (<kickmsg>) : Kicks user with optional kick message
*  /save : Manually save map to disc
*  /ctp <x> <y> <z> : Teleport to coordinates (eg. /ctp 100 100 100)
*  /tp <nick> : Teleport yourself to <nick>'s position
*  /tp <nick1> <nick2> : Teleport <nick1> to <nick2>
*  /reload : Reload admins and configuration
*  /give <nick> <id/alias> (<count>) : Gives <nick> <count> pieces of <id/alias>. 
                                        count = 1 is used if it is not provided.
                                        Support for over 64 items. Aliases configurable with item_alias.cfg
  * /rules <nick> : Shows server rules (from rules.txt) to <nick>
 
Compiling
---------
 
Depends on (and tested with):

 * zlib 1.2.5 (http://www.zlib.org)
 * libevent 1.4.14b (http://monkey.org/~provos/libevent/)
 * lua 5.1.4 (http://www.lua.org)

Compiling using linux (make & gcc):

 * Download and extract source
 * Go to mineserver/src/ directory
 * Run make
 * Run server with ./mineserver
  
Compiling using windows (VS2010):

 * Instructions coming soon...
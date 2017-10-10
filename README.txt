Awa es un blockchain Palmera basada en NXT

El objetivo de AWA es crear una plataforma abierta que pueda ser usada para 
todo tipo de procesos colaborativos y de negocio.

Esta basada en el nxt-blockchain kit y todo su codigo es abierto.

Se hara una distribucion inicial del AWA entre tod@s los Palmer@s que lo quieran.

Technical details:

The Nxt software is a client-server application. It consists of a java server
process, the one started by the run.sh script, and a javascript user interface
run in a browser. A JavaFX UI is also available and starts automatically on
supported configurations. To run a node, forge, update the blockchain, interact
with peers, only the java process needs to be running, so you could logout and
close the browser but keep the java process running. If you want to keep
forging, make sure you do not click on "stop forging" when logging out. You can
also just close the browser without logging out.

The java process communicates with peers on port 7874 tcp by default. If you are
behind a router or a firewall and want to have your node accept incoming peer
connections, you should setup port forwarding. The server will still work though
even if only outgoing connections are allowed, so opening this port is optional.

The user interface is available on port 7876. This port also accepts http API
requests which other Nxt client applications could use.

The blockchain is stored on disk using the H2 embedded database, inside the
nxt_db directory. When upgrading, you should not delete the old nxt_db
directory, upgrades always include code that can upgrade old database files to
the new version whenever needed. But there is no harm if you do delete the
nxt_db, except that it will take some extra time to download the blockchain
from scratch.

The default Nxt client does not store any wallet-type file on disk. Unlike
bitcoin, your password is the only thing you need to get access to your account,
and is the only piece of data you need to backup or remember. This also means
that anybody can get access to your account with only your password - so make
sure it is long and random. A weak password will result in your funds being
stolen immediately.



# **Design Goals**
## Table of Contents
 - [I. The Server](#i-the-server)
 - 

## **I. The Server** 
> Nautrally, the server itself is the main focus of this project. I plan on making this server as stable as possible, and ensuring minimal maintenence is required to keep the server running indefinitely. Something this complex is going to need some ground rules.

**1. The server should stay running indefinitely.** In general, the server should only go down if absolutely nescessary, e.g. when the game version is updated, a mod/plugin needs a security update, et. cetra.
<br>
<br>
**2. The Server should not be reliant on any specific "external" software.** If the server is to remain running indefinitely, it should avoid introducing major "dependencies". This means:

 - **The server will be FULLY vanilla compatible.** For example, I should we able to switch the server to a vanilla jar at any time without anything breaking. *Yes, this means we should avoid Bukkit/Spigot/Paper/*[your favorite fork here]. Sorry. By using software maintained by an external dev team, the server may run into problems when a game update releases, or a critical vulnerability of some sort is discovered.
 - **No changes to the vanilla game's mechanics.** Again, the goal is for *anyone* to be able to hop in and play whenever they want, forever. If we want that to happen, the server must not require any more effort to play than the vanilla, unmodified game. While *client-side* modpacks, QoL improvements, etc. will be provided, it will never be *required.* While the first rule implicitly prohibits any changes to core gameplay, it is vital that this stays true all thoughout the server's construction - so no custom datapacks, combat, world gen, etc.

 In short, if it changes anything about vanilla minecraft gameplay, we should avoid it. Someone who has only played Vanilla minecraft for the last decade-or-so should be able to join the server and have everything function just as they expect -- So no unnesscessary bug "fixes" either. *There may be some exceptions to this, but I'll try to get everyone to agree to fix/change/remove anything like that if/when they arise.*
<br>
<br>
**3. Keep the server lightweight!** Any modifications to the vanilla jar should be limited to performance improvements (which **don't violate rule 2**).
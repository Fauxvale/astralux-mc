<p align=center>[pretty image here]</p>

# **Design Goals** 
> Naturally, the server itself is the most important part! I plan on making the server as stable as possible, and ensuring minimal maintenance is required to keep the server running. 

**1. The server should stay running indefinitely.** In general, the server should only go down if absolutely necessary, e.g. when the game version is updated, a mod/plugin needs a security update, et. cetera. I plan to keep the server running indefinitely, never resetting the world (unless we really want to). Even if I lose interest and don't play for 6 months, I will try to keep the server up and running on the latest version of Minecraft 24/7 with as little fus as possible. 
<br>
<br>
**2. The Server should not be reliant on any specific "external" software.** If the server is to remain running indefinitely, it should avoid introducing major "dependencies". This means:

 - **The server will be FULLY vanilla compatible.** In essence, I should be able to switch the server to a vanilla jar at any time without anything breaking. Yes, this means I'll be avoiding Bukkit/Spigot/Paper/*[your favorite fork here]*. Sorry. By using software maintained by an external dev team, the server may run into problems when a game update releases, or a critical vulnerability of some sort is discovered. Things take time to update; projects get abandoned.
 - **No changes to the vanilla game's mechanics.** Again, the goal is for *anyone* to be able to hop in and play whenever they want, forever. If we want that to happen, the server must not require any more effort to play than the unmodified vanilla game. While *client-side* modpacks, QoL improvements, etc. will be provided, it will never be *required.* While the first rule implicitly prohibits any changes to core gameplay, it is vital that this stays true all throughout the server's construction - so no custom datapacks, combat, world gen, etc.

 TL;DR if it changes anything about vanilla minecraft gameplay, we should avoid it. Someone who has only played Vanilla minecraft for the last decade-or-so should be able to join the server and have everything function just as they expect -- So no unnecessary bug "fixes" either (i.e. all farms should work!). *There may be some exceptions to this, but I'll try to get everyone to agree on changes before taking action should the need arise.*
<br>
<br>
**3. Keep the server lightweight!** Any modifications to the vanilla jar should be limited to performance improvements (which *don't violate rule 2*). In order to cut down on excess resource consumption, as of 4-11-23, **the server will run [Fabric](https://fabricmc.net/).** Fabric was chosen due to its quick updates, performance, and solid community of developers. At some point I may switch over to [Quilt](https://quiltmc.org), but it's not *quite* stable enough for production (according to the QuiltMC devs themselves).
<br>
<br>
**4. Long-term projects require long-term solutions.** I don't want the server to fall victim to my own stupidity. The server will keep backups (and backups of those backups) all on it's own. I've rented out an AWS "S3" Storage Server to make sure they stay safe. As of writing, I'm still hosting the panel/server itself on an Oracle Cloud "Free Tier" Server, but I've set things so I'll be able to migrate to a ""real"" VPS if anything goes wrong. Speaking of which; While I tend to prefer open-source applications for my personal projects, I've elected to move away from [Pterodactyl Panel](https://pterodactyl.io/) in favor of [AMP](https://cubecoders.com/AMP) by [CubeCoders](https://cubecoders.com/) *(also known as "Application Management Panel", the most bland and forgettable name ever).* This was a tough decision for me, as AMP is a *closed-source, paid software! \*gasp\**

I feel the cost will be worth it though, as AMP has good customer support and a VERY large userbase. If something goes wrong, it's pretty much guaranteed to be dealt with quickly and easily (many large server networks use AMP, and some pay $200+ subscriptions, so failure is not an option 💀).
<br>
<br>
*..and last but not least,* <br>
**5. Be excellent to each other!** This document may present things in a semi-formal manner, but please never forget that this is supposed to be for fun! This is literally "just a game", so please do your part and keep it fun for everyone else.
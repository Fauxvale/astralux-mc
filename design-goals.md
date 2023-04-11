<p align=center>[pretty image here]</p>

# **Design Goals**
>   #### *The risk I took was calculated, but man, am I bad at math...*
>

**1. The server should stay running indefinitely.** In general, the server should only go down if absolutely necessary, e.g. when the game version is updated, a mod/plugin needs a security update, et. cetera. Additionally, I'll never reset the world (unless everyone really wants to). *Even if I myself lose interest and don't play for 2 months, I will try to keep the server up and running on the latest version of Minecraft 24/7/365 with as few issues as possible.*
<br>
<br>
**2. The Server should not be too reliant on any external software.** If the server is to remain running indefinitely, we should avoid introducing extra "dependencies". This means:

 - **The server will always be FULLY vanilla compatible.** In essence, the server will remain 100% intact even if it's switched to the vanilla server jar *with zero corruption/missing functionality*. This means I'll be avoiding Bukkit/Spigot/Paper/*[your favorite fork here]*. Sorry. If the server uses any external plugins, we could run into problems very quickly when a new Minecraft update releases, or random plugin developers decide to vanish without warning.
 - **No changes to the vanilla game's mechanics.** Again, the goal is for *anyone* to be able to hop in and play whenever they want, forever. If we want that to happen, the server **must not require any more effort to play than the unmodified vanilla game.** While client-side modpacks & QoL improvements will be provided, they will never be *required.*

 **TL;DR** *I'll avoid major gameplay changes & "vanilla" clients will always be able to connect.*<br>
**This includes keeping bugs/exploits that have a legitimate use case *(and can't be used for evil  👺)* intact!** For example, most exploits commonly used/abused by the technical minecraft community will stay -- *within reasonable limits.* There will always be *some* exceptions to this rule, but I'll try to get everyone to agree on changes before taking action should the need arise.
<br>
<br>
**3. Keep the server lightweight!** Any modifications to the vanilla jar should be limited to performance enhancements or minor QoL tweaks *(which don't violate Rule #2*). As of 4-11-23, **the server will run [Fabric](https://fabricmc.net/).** Fabric was chosen for its solid userbasse, fantastic performance and quick updates. At some point I may switch over to [Quilt](https://quiltmc.org), but it's not stable enough for live production yet (according to QuiltMC devs themselves).
<br>
<br>
**4. Long-term projects require long-term solutions.** I don't want this server to suffer from outages, exploits, or my own stupidity. The server will keep backups (and backups of those backups) all on it's own. I've rented out an AWS "S3" Storage Server to make sure they stay safe. As of writing, I'm still hosting the panel & server itself on a remote VM via Oracle Cloud's "Free Tier", but I've prepared it in a way that I'll be able to migrate to a more reliable service should the need arise. Speaking of which; While I tend to prefer open-source applications for my personal projects, I've elected to move away from [Pterodactyl Panel](https://pterodactyl.io/) in favor of [AMP](https://cubecoders.com/AMP) by [CubeCoders](https://cubecoders.com/) *(also known as "Application Management Panel", the most bland and forgettable name ever).* This was a tough decision for me, as AMP is a *closed-source, paid software! \*gasp\**

I feel the cost will be worth it though, as AMP has good customer support and a VERY large userbase. If something goes wrong, it's pretty much guaranteed to be dealt with quickly and easily. Many large server networks use AMP, and some pay $200+ subscriptions, so failure is not an option for them 💀
<br>
<br>
*..and last but not least,* <br>
**5. Be excellent to each other!** These docs might look intimidating, but please never forget that this is supposed to be for fun! This is literally "just a game", so please do your part and keep it fun for everyone else. ❤️

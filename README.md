# Minecraft: Gear VR Edition — Quest 3 Compatibility Patch

This is a patched version of Minecraft: Gear VR Edition `1.16.40.02`, made to work again on the Meta Quest 3 after a HorizonOS update caused the original game to crash immediately after opening.

## What has been fixed?

- The game boots properly on current HorizonOS instead of immediately crashing.
- You do not a controller paired via Bluetooth anymore, the Touch controllers will work. There aren't as many buttons, however, so you will want to go into your Settings and rebind the buttons.
- It will also no longer stop you from booting the game if it doesn't detect a controller or your Touch controllers.
- Microsoft/Xbox sign-in works through a browser window inside the game. No separate Smart Glass or Xbox app required.
- Signed-in account persists across closing and opening of the app.
- Due to the way the patch was written, 'Steve' would always appear over your avatar. This was patched to show your GamerTag as normal.
- The Marketplace loads, shows the correct Minecoin balance, and allows downloads. I did not attempt to spend Minecoins on anything or buy new Minecoins. If you test it, let me know if it works!
- Xbox achievements work and sync to your profile.
- Friends and their online status appear correctly.
- LAN multiplayer works when both devices are running Minecraft `1.16.40.02` on the same network.
- Gear VR can not join a LAN game via the Online Friends tab. When a friend is hosting on the same LAN subnet and pops up in your Online Friends list, their world will be added automatically to the bottom of the Servers tab. The saved entry is only refreshed if their address changes.
- I tested this with a Quest 3 and the Windows version of 1.16.40.02 playing together. I don't have two Quest headsets to test it with. If you test it, let me know if it works!
- Gear VR can also host a LAN world, which appears normally on the matching Windows version during my testing.

## Installing it

Install the latest version if the Releases section through SideQuest or ADB like any other sideloaded APK. Because it has been modified, it uses a different signature from the original game. If Android reports a signature conflict, uninstall the old copy first and then install this one.

Uninstalling or clearing the app will erase its settings, downloaded content, locally stored worlds, and saved sign-in. Back up anything important first.

## Signing in

Press **Sign In** inside Minecraft and complete the Microsoft login window. You may briefly see a “Connecting” screen afterward. If it remains open, back out of it and check the main menu. The best signs that login actually worked are:

- Your GamerTag appears.
- The Marketplace shows your Minecoins.
- Your friends list loads.
- The Achievements screen loads your Xbox achievements.
- The "Sign In" button disappears.

I tried making this a little less janky, but ended up giving up on this part. I may revisit it at a later time. For now, it works. And only like 12 of you are going to use this anyway probably.

## Multiplayer

LAN play requires both games to be on the same Minecraft version and the same local network. This patch was tested with Windows Bedrock `1.16.40.02` and Gear VR `1.16.40.02`.

Internet play across two different networks is **not fixed yet**. Port forwarding, direct public addressing, IPv6, or a virtual-LAN service may provide a path forward, but none of those options are included in the current build. This is something I want to get working, but it will likely take a substantial amount more time, and I'm currently burned out on this and need a little bit of a break.

## Remaining quirks

- The first-login/“Connecting” windows can occasionally be a little clunky.
- Some old cloud characters may fail to load. Creating a fresh character inside this version worked during testing. If you are having problems with crashes when it's loading your avatar's costume, you may need to open up a newer edition on a different platform to erase all of your saved characters there to prevent the Gear VR Edition from trying to pull them down. Saved Characters beyond 1.16.40.02 will probably cause problems. (It is likely possible to patch out the loading of Avatar Costumes completely. If enough people express interest in this, I will look at patching it.)
- Characters created here did not sync to other\newer versions of Bedrock. Tested with the Nintendo Switch Edition.
- The achievement screen may incorrectly show `Time Played: 0 Hours`, even though achievements themselves work and sync correctly. (Another thing I may look at patching at a later time.)
- LAN worlds hosted by Windows may not appear in Gear VR’s normal LAN list. The automatically created `AutoFriend-...` entry in the Servers tab is the workaround.
- The automatic server entry needs a Microsoft account sign-in to discover a friend’s current address. A previously saved entry may continue working without sign-in as long as the host’s address has not changed.

## Current status

For now, the important stuff works: the game launches, Microsoft/Xbox login works, the Marketplace works, achievements unlock, and local multiplayer works in both directions.

Enjoy. It was a lot of effort. Hopefully Microsoft doesn't decide to break my patches at some point.

Alec Breen | TheBreenis

# bnsnogg

I've had some time, so I decided to update my gameguard bypass for bns - well, because gameguard is shit and I want to send a message to NCSoft that their Gameguard is shit, their policy about banning people based on email domains is shit, their policies at all are shit too.

Also decided to release it here (only in binary form, there won't be any source code, don't even try requesting it!)

Downloads are here: https://github.com/Evengard/bnsnogg/releases

Version 2.0.4 is for x64, 2.0.3 is still displayed for old x86.

Among the core action of actually disabling GameGuard (Also prevents aegisty.bin to be loaded too), this also have some nice features, such as:

1 Multi-instances on same machine (open as many clients at the same time from the same machine until your PC fries)

2 Launch the game without the launcher (and without the need to patch any config.dat-s or stuff - basically no files modifications needed) - just run it such as: 

    Client.exe /LaunchByLauncher /SessKey:"" /MacAddr:"" /UserNick:"" /CompanyID:"0" /ChannelGroupIndex:"-1" /ServerAddr:" " /StartGameID:"BNS" /RepositorySub:" " /GamePath:"" /LoginMode 2 /noweblaunching

(won't work without the antiGG)

3 Ability to override the config.dat loaded by config2.dat (config64.dat by cnfig642.dat) (say, you still want to change something inside it so it would persist updates) - just add the "/configdatoverride" switch

4 Persist acrss updates - no need to do anything after a client update - should work out-of-the-box (except some rare cases).

Works with NA/EU, may work as well on TW/JP, maybe even KR, but untested.

# INSTALLATION

Installation is very easy: just unpack all the files in the archive into the core directory you have BnS installed (where there is folders bin and bin64). After that launch as usual (through the launcher) or use the no launcher method above.

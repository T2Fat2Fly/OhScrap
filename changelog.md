KERBALCHANGELOG
{
	showChangelog = true
	modName = Oy!Scrap!
	license = Expat/MIT
	author = magico13, severedsolo, zer0Kerbal
	VERSION
	{
		version = 2.2.0.0
        versionDate = 19 JuL 2021
        versionKSP = 1.12.1
		versionName = Final Countdown...
		CHANGE
		{
			change = Code
			subChange = recompile for KSP 1.12.1
			subChange = use .net 4.7.2
			subChange = use C# 9.0
			subChange = update to Version.tt [v2.0.0.0]
			subChange = pull upstream changes from severedsolo (thank you)
		}
		CHANGE
		{
			change = Update
			subChange = usual spring cleaning and automation
			subChange = folder structure
			subChange = to modern back-end automation
		}
	}
	VERSION
	{
		version = 2.1.1.1
        versionDate = 02 Jun 2021
        versionKSP = 1.9.1
		versionName = More ways to Fail, and more Kerbals allowed to fix it (part II)
		
		CHANGE {
			change = Repair
			subChangee = fix Icon.ping (issue #11) by moving it where it should be
			subChange = other minor housekeeping items
		}
		
		CHANGE {
			change = Update
			subChange = changelog to modern KerbalChangeLog standards
			subChange = 
		}

        CHANGE {
            type = Changed
            change = Back end  
            subchange = add auto JSON  
            subchange = update automation to latest version  
            subchange = start working with yaclog-KSP (thank you cineboxandrew!)
        }
	}
	VERSION
	{
	  version = 2.1.1.0
	  versionName = More ways to Fail, and more Kerbals allowed to fix it
	  change = folder restructuring
	  change = improved workflow
	  change = added 'Validate AVC .version files' workflow by @ DasSkelett (thank you @HebaruSan)
	  added CONTRIBUTING.md
	  added htm versions of Readme.md CONTRIBUTING.md to root
	  included Readme.htm in future release
	  internal automation updates
	  CHANGE
	  {
		change = Allow 'Mechanics' from USI to affect effets
		subchange = suggested by @dirk
		subchange = current code allowed Engineers (and only Engineers) a bonus to repairs
		subchange = adjusted code to allow any Kerbal with the "FailureRepairSkill" to receive a bonus to repairs
		subchange = FailureRepairSkill is a Stock skill that all Engineers have
		subchange = added a patch that adds FailureRepairSkill to USI MKS Mechanics
		subchange = easy to add "FailureRepairSkill" to other careers if requested by users
	 }
	 CHANGE
	 {
		change = New parts can fail!
		subchange = Implement engine under-thrust/under-Isp failures in a way that doesn't depend on thrust limiter.
		subchange = thank you to @bfrobin446
		subchange = ~~code from TestFlight~~ (thank you	@Agathorn @linuxgurugamer and et al)
		subchange = ~~section covering this code (CC BY-NC-SA 4.0) inserted into license file~~  
	 }
	 CHANGE
	 {
		change = Speed up new code
		subchange = thank you to @Lisias
		subchange = reset repository/code to 2.1.0.0
		subchange = updated to faster version of new EngineModuleWrapper.cs
		subchange = new code subject to GitHub ToS and to existing OhScrap License (MIT)
	 }
	 CHANGE
	 {
		change = Post Beta changes
		subChange = [BUG 2.1.0.0b] corrected 'Engineer' patch (was adding, not modifying FailureRepairSkill)
		subChange = [BUG 2.1.0.0a] Icon.png moved from /Plugins/ -> /Plugins/Textures/ to correct 
		subChange = [BUG 2.1.0.0c] moved "/GameData/OhScrap/PluginData/DefaultSettings.cfg" -> "/GameData/OhScrap/Plugins/PluginData/DefaultSettings.cfg"
		subChange = [BUG 2.1.0.0d] split game.settings into two columns for readability and allow for future expansion
		subChange = [BUG 2.1.0.0d] added bool ColoredPAW = treu to game.settings for future use
		subChange = [BUG 2.1.0.0e] corrected with a ^t (Alternators)
		subChange = [BUG 2.1.0.0f] added in tooltips and descriptive text
	}
	CHANGE
	{
		change = Bug Status
		subChange = [D][NEW][BUG 2.1.0.0a] Texture resolution is not valid for compression: 'GameData\OhScrap\Plugins\Icon.png' - consider changing the image's width and height to enable compression
		subChange = [D][NEW][BUG 2.1.0.0b] ExperienceSystemConfig: Experience trait 'Engineer' already exists, and trying to add a duplicate Effect of 'FailureRepairSkill'
		subChange = [D][NEW][BUG 2.1.0.0c] "/GameData/OhScrap/PluginData/DefaultSettings.cfg" not found
		subChange = [D][NEW][BUG 2.1.0.0d] Too much information in Game.Settings page that it needs to scroll; needs reorganization
		subChange = [D][NEW][BUG 2.1.0.0e] typo: game.settings Alernators
		subChange = [WIP][NEW][BUG 2.1.0.0f] game.settings could use better/more explanation for what the settings are for
	}
  }
  VERSION
  {
	  version = 2.1.0.0
	  versionName = new maintainer, same great taste!
	  change = recompile for KSP 1.9.1
	  change = recompile with .NET 4.8
	  change = folder restructure
	  change = added version.tt / AssemblyVersion.tt
	  change = adjust .csprog to zer0Kerbal
	  change = adjust autobuild/deploy process to zer0Kerbal
	  change = added Logger.cs
	  change = use Version.Number from tt processes
	  change = adjusted log path from /severedsolo/OhScrap/Logs/ to /OhScrap/Logs/
	}
	VERSION
	{
		version = 2.0.1
		change = Fix NRE Spam and Slowdown
	}
	VERSION
	{
	version = 2.0.0.1
	change = Fix bad JSON in .version file
	}
	VERSION
	{
		version = 2.0
		change = Recompile against KSP 1.8 / .Net 4.2.7
		change = Resized icon so KSP can properly compress it when using half res textures
		change = Added Alternator Failures
		change = Added Landing Gear Failures
		change = Support MADLAD's Install Validator
	}
	 VERSION
	{
		version = 1.7.1
		change = Fix SRBs constantly spamming message app on failure
	}
	 VERSION
	{
		version = 1.7
		change = Fixed RCS thrusters being allowed to fail when RCS is turned on
		change = Parachutes will now only fail while deployed
		change = Fixed an NRE that could occur when other mods apply MM patches after the Failure Module has attached itself to a part.
		change = Failure Modules will now cache all modules they need to interact with, instead of grabbing them on each FailPart() call.
		change = timeBetweenChecksRocketsSpace has now been split into timeBetweenChecksLocalSpace (Homeworld or its Moons) and timeBetweenChecksDeepSpace (everywhere else)
		change = timeBetweenChecksLocalSpace reduced to 20 minutes
		change = timeBetweenChecksDeepSpace increased to every roughly every 7.5 hours.
		change = Fixed an issue where SRBs would not post failures to the Messages App or Log they had happened.
	}
	 VERSION
	{
		version = 1.6.3
		change = Force Editor Ship cache to refresh when it gets itself into an invalid state.
	}
	 VERSION
	{
		version = 1.6.2
		change = Fixed issue where Editor Ship was being cached before it had any parts.
		change = UI will now point out that the Editor Ship has no parts, rather than just reporting Safety Rating 0.
	}
	 VERSION
	{
		version = 1.6.1
		change = Fixed Typos in ParachuteFailureModule.cfg
	}
	 VERSION
	{
		version = 1.6
		change = SEVEREDSOLO: Fixed DivideByZero exception in Editor when no FailureModules were actually present on the craft.
		change = SEVEREDSOLO: Removed unnecessary onEditorShipModified event. All Safety Ratings are now calculated in Update() instead.
		change = ALL OTHER CHANGES BY NIPPERYSLIPPLES
		change = Remote tech antennas can now fail, will only do so when deployed (you can pack backups) and will show as properly malfunctioned when they are failed.
		change = Antenna Failures no longer happen if commnet is disabled (they previously happened, but did nothing except add highlight).
		change = Minor performance improvements in several Failure Modules.
		change = Fixed repairs not being available in some situations.
		change = Mod will no longer Spam NRE's if FAR is installed and Control Surface Failures are enabled.
		change = Added ModWrapper class to facilitate FAR and RemoteTech compatibility.
		change = AntennaFailureModule will no longer be added to parts if RemoteTech is installed.
		change = ControlSurfaceFailureModule will no longer be added to parts if FAR is installed.
		change = Added support for FAR and FAR's implementation of RealChute. See https://github.com/severedsolo/OhScrap/pull/18 for details.
	}
	 VERSION
	{
		version = 1.5.1.2
		change = Changed the license in the Github repo back to MIT
	}
	VERSION
	{
		version = 1.5.1.1
		change = Rerelease due to not shipping the DLL
	}
	VERSION
	{
		version = 1.5.1
		change = Recompiled against KSP 1.6.1
		change = Fixed SRBs rolling 4-5 times before launch (which was leading to the abnormally high failure rates)
		change = Fixed all parts automatically being tested because apparently vessel.speed is not relative to the vessel.....
		change = Fixed SRB safety ratings not really reflecting the parts likelyhood to fail.
		change = Fixed invalid characters in EngineFailureModule patch
		change = Fixed Space Engine (Terrier etc) always having a Safety Rating of 1 and simultaneously being physically capable of failing.
		change = Logger will create Logs directory if it doesn't exist
		change = Slightly reduced baseFailureChance of SRBs
	}
	VERSION
	{
		version = 1.5
		change = Recompiled against KSP 1.6.0 (1.5.x should continue to work fine)
		change = Fixed issue where failure rolls would be spammed in prelaunch
		change = Exposed baseFailureChance and expectedLifetime for Space Engines in the MM config for EngineFailureModule
		change = Added bash script to automate release build process (only relevant if you are compiling from source, but it's in the Github Repo so mentioned it here)
	}
	VERSION //Declares a version node
	{
		version = 1.4.2 //Version number, numbers only with no spaces!
		change = Fixed SRBs being allowed to fail during KRASH simulations (for real this time)
	}
	VERSION //Declares a version node
	{
		version = 1.4.1 //Version number, numbers only with no spaces!
		change = Fixed SRBs being allowed to fail during KRASH simulations
	}
	VERSION //Declares a version node
	{
		version = 1.4 //Version number, numbers only with no spaces!
		change = CKAN USERS ONLY: Kerbal Changelog by Benjamin Kerman is now a required dependency
		change = MANUALLY INSTALLED USERS: Kerbal Changelog by Benjamin Kerman is bundled as an optional (but recommended) mod.
		change = Recompile against KSP 1.5.1 
		change = Failures will no longer be calculated per part. Instead, we'll take into account the overall reliability of the vessel, and use that to determine failure rates. (Ie, if you stick a bunch of really good parts on your rocket, and one really crappy one, the rocket will still be less prone to fail than one with all crappy parts). A really cool side effect of this, is that if you stage away your bad parts, your vessel will become more reliable overall (ie, you can have a bad launch vehicle, but a tried and tested payload, and once the launch vehicle is gone, the payload will be uber reliable).	
		change = Failures will be rolled for constantly (but rate limited) instead of just on loading the vessel. At the moment, it's every 10 seconds in atmosphere for the first two minutes, every 2.5 minutes after that while in atmosphere (known as "plane mode") and every 30 kerbal minutes out of the atmosphere - to simulate the fact that things are much more likely to go wrong on launch.
		change = All of the above parameters can be edited in DefaultSettings.cfg which is located at OhScrap/PluginData
		change = Parts can only fail if they are actually in use (ie engines firing, Reaction wheels turning, etc) - this may have been technically in the last version, but I found a bunch of places where it wasn't actually turned on. 
		change = Overall rebalance of the reliability system
		change = Remote Repair has been reduced to a 20% chance of success, EVA to 40% and engineers will give a 10%*their level boost to the repair chance (so a Lv5 Engineer will give you a 90% chance of repair on EVA). 
		change = MASSIVE code cleanup - handling the failures on a per vessel, rather than per part basis means less garbage, better performance and easier for me to maintain etc. I've also moved a BUNCH of duplicated code into their own common methods. 
		change =	Parts that have not been tested/launched can now be recovered. The tradeoff for this is that those parts will receive NO bonuses for recovery. Ie, it will still have the failure rate of a "fresh off the factory line" part. 
		change =	Parts that have not been tested/launched can now be recovered. The tradeoff for this is that those parts will receive NO bonuses for recovery. Ie, it will still have the failure rate of a "fresh off the factory line" part. 
		change =	Randomisation is gone. Parts will have standard failure rates. 
		change =	Safety Rating system now runs from 1-10 rather than 1-5 
		change = Safety Ratings are now relative rather than absolute (ie it's linked to the parts base reliability, not a fixed number)
		change = Mod will log to the OhScrap/Logs folder
		change = "Extra Logging" option will show you every roll and a guess at the probability of a part failing in the next 2 minutes/15 minutes/30 days (depending on the Vessels Situation). Note that this can be inaccurate in some situations.
		change = You can also see this information in the UI by creating an empty text file called debug.txt in the Oh Scrap Directory (all lower case if your OS cares about such things)
		change =	Probably a bunch of other stuff I'm not remembering right now. 
		change = Added option to override Stage Recovery and recover parts but no funds. Please note this is highly experimental and may not even work at all.
	}
}

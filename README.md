【Sorry, my English is no good. So only with the help of translation tools ...】

--------------------------------------------------------------------------------------

Mod Name: Time Is Money

Workshop: https://steamcommunity.com/sharedfiles/filedetails/?id=2045438856

Introduction:

	1/ Add deposits to players @banking account according to online time (reward every n minutes)
	2/ You can customize the reward interval and how many deposits are rewarded each time, and write some events to the record file.
	
Special note:

	1/ Server must already have the required mod: @ banking
	2/ Each player's time is calculated separately.
	   Players enter the server to start calculating time, exit the server to clear the time and stop calculating.
	   
Config File:

	path：    DayZServer\Profiles\xxxxxx\S1mpleTAT\Time Is Money\TimConfig.json
	parameters:
		<1> "Reward_Interval"  // Interval of each reward, in minutes. Higher values are more conducive to server stability.
		<2> "Reward_Value"     // How much to reward each time. (Add directly to the players @banking account.)
		<3> "Record_Reward"    // Switch of reward record, 0=no record / 1=record.
		<4> "Record_Other"     // Switch of other record, 0=no record / 1=record.
		<5> "Record_Language"  // Language for logs,  "cn"=chinese / "en"=english
	Tips:
		1/ If "Reward_Interval" = 0, No rewards will be given to any player!
		2/ If you change "Reward_Interval", you must restart the server to take effect.
		3/ change "Reward_Value" / "Record_Reward" / "Record_Other" / "Record_Language"  No server restart required.


Logs File:

	After the server is started, "Reward" and "Other" folders will be generated automatically.
	And according to the year - month - day, the .log file is automatically generated.
	
	Reward:
		Record path:    DayZServer\Profiles\xxxxxx\S1mpleTAT\Time Is Money\Logs\Reward
		Record event:    player will record every time they get a reward.
		
	Other:
		Record path:    DayZServer\Profiles\xxxxxx\S1mpleTAT\Time Is Money\Logs\Other
		Record event:    Every time the player enters or exits the server.
		
Known problems:

	Because the server's archive is used,
	the first time a new player enters the server will have no effect.
	Solution:  the players exits the server and enters again.

Copyright：

	I do not give permission to distribute, repack, 
	reupload or modify this mod in any way without my permission.

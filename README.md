# Basic_MBR_parser 0.1.0 - Basic Forensic tools
this tool contain that parsing Bootcode, partition table and signature.
but not offer carving operation.

to be update!!!
good afternoon, good evening, and good night.
@@@@@@@@@@@@@@@@@@@@@@@#$$###$$$#####$##$$##@@#@#@#@@#@@###$$$==$$$$##@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@#$$###$$$$#$$$$$$$$###@@@@@@@@#@##@##$=$$$$$$$$##@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@#$$##$$$$#$$$$$$$$$##@@@@@#@@########$$==$$$$$$$$#@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@#$$$#$$=$#$$$$=$##$####@@@##########$$$====$$$$$$$##@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@##$$#$$==$$=$$$$#########@##$$######$$$$$=====$$$$$$#@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@#$$$$===$==$$$=######$####$#$$#$$$#$$$======$$=$$$$$$#@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@#$$$$=======$$=###$##$$###$$$=$$$==#$$$===$======$$#$$$#@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@##$=$===$====$$$$$$$$$=$$$$====$=$$==$====*========$##$$$#@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@#$=========$$=$$$$=$=$======*=*==$$=*$=============$$##$$#@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@#$==============$=======***==*****==***============$$=$$$$#@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@#$$=$$==========*********!!!**!!**!******=*==========$=$$$$$#@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@$===$========*******!!!!!!!;!!;;!*!!!!*!*****========$=$$#$##@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@#===$$==*==*=***!!!*!;;;!!;;;;;;;;!;;;!!!!!****=======$$$$#$$#@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@====$$====******!;;!;;;:!!;::::;::;;;;;;!!!*****=====$$$$$$$$##@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@#===$$==*=****!*!;::;::;:!;::::~;:~:;:;;:!!!!*!!*=====$$$$#$$$$#@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@$=$$=$===***!!**!;::;~::~!;:::~~:~~~:::::!!!!*!!**====$$$$#$$$$#@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@#$$$$=====**!!;**;:~::~~~~;::~~~-~;~~::~:::!!!*!!!*===$$$$$$$$$$#@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@#$$$======*!;;;**;~~~:-~~:;~~~~---:~~~::~::;!!!!!;!===$$$$$$$$$$#@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@#$$$=======*;;:;*!;~-~:---:;::~~---~~-~~~~::;;;;;;;!*==$$$$$$$$##$@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@#$$$=======!:;:;!!:~--~---::::~---,-~~-~~~~~:;;;;;;!*==$$#$$$$$$##@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@#$$$====$==!~!:;!!:-,-~---:::~----,,-~---~~~::;;;;;!!===$$$$$$$$##@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@#$$=====$$*:~;;;::-,.,---~~;:~~-,,,,------~~~::::;;!!===$$#$$$$$##@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@#=========*::;;:~-,...-~--~;:~~-,,,,,-----~~~~~~:;;;!*==$$#$$$$$##@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@#=====*===!~:;:-,,....,---:~~--,,..,,,-------~~~~::;!*==$$$$$$$$#$@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@#==$==*===;~:;~,,......----~--,.....,,,,------~~~~::;*===$$$$$$$$$@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@#$=$$=**=*;~:~-,......,--,,,,,......,,,--------~~~::;!====$$$$$$$$#@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@$$$==****:---,,,,...,,,,,,,,,,..,,,------~~----~~:::;*===$$$$$$#$@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@$$$===**!~,,,,,------~~~~~--,,.,--~~:::::::::~~~~~::;*====$$$$$#$@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@#$$$$==*;-,,,-~:;:;;;!!!!;:~--,--::;!!**!!!!!!;::::::!====$$$$$#$@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@$$=$$=*:-,,-:;!!!**===*!;:~~-,-~:;!**===******!;::::;*===$$$$$$$@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@#$$$$=*:,,-:;!;!!!!***!!;::~,,-~:;!!***!!!**==**!;::;*==$$$$$=$$@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@#=$$$=!~,,~;;;:~~~~~~::;;:~-,,-~;;!!;:::::;;!!**!;::;*==$$==*!=$@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@$;=$$=!~,,~::~~~~~~:::;;::~,..-~;;!;;;!!!!!!!;!!!!;::*==$$=*!!*@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@$:;*==!~--~~~~~:;!!!***!;:~,..,~:;!!!***===**!;!;;;::!==$=*;;!!@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@$~~!==!~----~~;!!!!!!*!!;:~,..,~:;!;;;;;;!!!*!!;;;;::!====;~:!;#@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@=--:==!-----~:;::::::::::--,..,~::;:::~~::;;;;;;:::::!*==!:::;;#@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@!-,-*=;-,------~~~~~:::~--,...,-~::::::::;;::~~~:::::;*=*;~~~::$@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@;-.-;*;-,,,,,---~:::::--,,,...,-~~~~~~~~~:~~-~~~~~:::;*=*;:;~~:$@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@;. .~*:-,,,,,..,,,,,,.........,,--~~--,,,,,,-,,--~~:::!**:!!:~~$@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@:..-:!:-,,,.... ...............,--~---,,,..,,,,---~~::;!!:;!;:~$@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@:.,-~;~,,,,...    .. ..........,-~~--,,,....,,,----~::::::;;;;~=@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@#~.,,,--,,,,..        .........,,-~-~~--,....,,,----~~::~:~:;;;~*@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@#-.,...--,,...     ...,,...,,.,,--~--~:~-,,,,,,,---~~~::~:::;;;:!@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@#-.,. .,-,,...    ..,-~-..,,,,-~~~~~-:;:~--,,,,--~~~~~::~:::;::~!@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@#-,,...--,,,.......,~~----~~--~~::::~:;;:~-------~~~~~::::~;:~~:!@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@:.....--,,,,,..,,-~~~-,-:;;:~~:;!*!;;;:::~~---~~~:~~~:::::;~-~:*@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@:,  ,,---,,,,,,---~~-,,-~~~~~:;!;;;;;:::::~~~~~~::::::~:;~~~~~~$@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@;,  .,---,,,,,--~~:~-,,,--~~:;;!!;;;::::::~~~~~~::::::::;;:~~:;@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@*,...----,,,,--~~:~-,,,,,---~:::;:::::::::~~~::::::::::;;;::::=@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@#-,,,----,,---~~~~~-,,,,,,,,---~~~~~~~:::::~:::::::::::;;::::!#@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@;,,,,---,-,-~~~~~--,,.....,,,---~~~~~~:::~~~~::::::::;!;::;*#@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@$~,,,---,---~~~~---,,,----~~~~:::;;;:::::~~~~~:::::::;;!!*=#@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@$;~~~--,---~-~~~---~~~---~~~~~:::::!;;;:~~~~~::~~~::;;$$$@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@##$:--------~~~~::-.,.,. ,, ~,-~~;*!;:~~-~~::~~:::;;#$@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@;------,-~~~;*:-.,    ,..-.,,-:!=!;~~--~::~:::::;#$@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@!~-----,-~-~:!-,.,,,--~--~~-~~:;!::~---~::~:::::;$$@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@=~---,,,,-,,-~~::!*=$$$$$##$=;::~~~~---~:::::::::=$@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@#:----,,,,,,.,~*$$##@@##$$$*!:~-~~----~~:::::::::=$#@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@;~-----,,,,,,,-~:;;!;;;:::~--~~~----~~:::::::::;$$##@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@*~-------,,,.,....,,,,,,,,---~~----~~:;::::;:::;##@###@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@#:~------,,..,........,---~~~~~~~-~~:;;;;;;;:::;#@@@###@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@*:~~~~---,,,,,,,,----~~::::~--~~~~::;;;;;;;:::;@@@@@#$#@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@#:~~~~~--,,,,,,,-----~~:~~~~-~~~~~:;;;;;;;;:::;@@@@###$@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@@=::~~~--,,,,,,,,,--~~~~----~-~~~:;;;;;;;;;::;;@@@@@##$$@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@@#!::~~--,,,,,...,,--~~---------~:;;;;;;;;;:::;#@@@@##$=$@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@#$=;:~~~--,,,.....,,-----------~~:;;;;!;;;;;:;;#@@@#@#$$$@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@=$=!::~~~-,,,......,,,---------~:;;;;!!;;;;;;;;#@@@####$$#@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@$===*:::~~~-,,,.....,,---------~::;;;!;;;;;;;;;!#@@@###$$$$@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@#===$*:~:::~~-,,,....,,-------~~~:;;!!!;;;;;;;;;!#@@###$$$$$@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@#$==$$=:~~:;::~--,,,,,,-------~~~::;!!!!;;;;;;;;;!$@@####$$$$@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@#$===$$=;~~~:;;:~--------~~~~~~~::;;!!!!;;;;;;;;;;!$@@@##$$$=$#@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@###$$==$$$$=!:~~:;;;:~~-----~~~~~~::;;!!!!!!!;;;;;;;;!!$#@##$$$$$$#@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@###$$$=====$$$$$!:~~::;;;::~~~~~:::::::;;!!!!!!!!!;;;;;;!!*$#####$$$=$#@@@@@@@@@@@@@@@@@@@
@@@@@@@##$$$$=$$$=$===$$$$*;~~~::;;;;;:::;;;;;;;!!!!!!!!!!!!!!;!!!!!*$##$$$$$$=$$#@@@@@@@@@@@@@@@@@@
@@@@#$$=======$$====$$$$$$$!:~~:::;;!!!!!!!!!!!!!!**!!!!!!!!!!!!!!!*=$##$===$$$$$$#@@@@@@@@@@@@@@@@@
##$====================$$$$*:~~~:::;;!!!!!*********!!!!!!!!!!!!!!!**=$#$$$$$==$$$$$$@@@@@@@@@@@@@@@@
*==============$=$====$$#$$=:~~~:::::;!!!!*********!!!!!!!!!!!!!!***=#$$==$$=$$$$$$=$#@@@@@@@@@@@@@@
===============$====$=$$==$$;:~~:::::;;!!!!********!!!!!!!!!!!!!***==$$$$$$$$$$$###$$$#@@@@@@@@@@@@@
=========$=====$========$$$$!::~~~~:::;;;!!!!!!!!!!!!!!!!!!!!!!!**=$$$$$#$$$$$=$##$$=$$=#@@@@@@@@@@@
===$==$$$====$========$$$$$$*;:::::~~:::;!!!!!!!!!!!!!!!!!!!!!!***=$$$$$$$$$=$$$##$$$$$$=$##@@@@@@@@
=======$=====$===$========$$=;;:::::~~~:;;;;;;!!!!!!!!!!!!!!*****=$$$$#$$$$$$$$$$$$$$#$$===$#@@@@@@@
======$$=$=$=====$=========$$!;;::::::~::;;;;;;;!!!!!!!!!!!*****=$$#$$$$$$$#$$$##$$$=#$$====$#@@@@@@
=======$======$=$$====$==$$$$=!;;:::::::::;;;;;!!!!!!!***!*****=$$$$##$$#$$#$$###$$$$$$$$=====$#@@@@
==*=$$=$========$$=========$$$*;;;;;;;::::;;!!!!!!!!**********=$$$$$##$$##$$$$#####=$##$$$======$#@@
=$==$=$$===$===$$=$===$$===$=$=!;;;;;;;;::;!!!!!!************=$$####$#$$$######$###$###$$$$=======$@
====$======$=$$$=$$======$$$==$=!!;;;;;;;;!!!!!!***********==$$#$#$$=##$$#$#$#####$$#$=$$==$$=======
===============$=$$==$===$==$$$=**!!!;;!!!!**!!*********===$$####$##$$#$$$####$##$$##$=$$$$$$$$====*
===========$$=$$=$$========$$=====*!!!;!!!*************==$$$$$##$$##$$$#$$#####$#####$$$=$$$=$$=====
=$$============$$=$===========$====**!!!!!********=====$$$$#$$$$$$$##$$#$$######$###$$$$$$$$=$====$=
=$$$===$======$$===$============$====***!!!******===$==$$$$#$$$$#$$###$##$##########$$$$$$$$=$====$=
=$$$====*$====$=!*=*=$!==**=*==**======*******======$$$$$#$$$$#$$#$$##$#############$$$$$$$$$$=$=$$=
$=$$$=:=~=:-!=$*;*=;*$,~=~;=~!=~!=$==$========$=$$$=$$$$####$$$####$#$$#######@@#$$$$$$$$$$$$=$=$$==
$=$$=*:=;=***$$=:;*;!=;:=!*=:!$*$$==$$$$$$$$=$$=$$$=$$$$#####$$####$#########@##$$$$=$$$$$$$$$$$===$
=$$$$==!;!!!!!!!;!!!!*;!=!;!=$=====$$==$==$$=#$=$$$$$$$$##$$#$##############@##$$#$$$$=$$$$$=$==$$=$
====***:.--,,-.~.~,--:,,:-,-*$=*=*=$$==$$$$$$$$$$$$$$##$############$######@@###$$$$#$$$$===$$===$$=
=$*!;;;=-::,,~.-,~-----,--.,!*!!!!!=$$$$$$$$$##$$$$$$##$$$##############@@@@##$$$$$$$$$===$=$===$$$=
===*!**$:!!;;!;:;!!!;;;;:;;;*******=$$$$$$$$$##$$$$$$##$$#############@@@@@##$$$$$$$$$$$$$$=$$$=$$$$
==$==$=$=====$*===========$$$=$$===$$==$$$#$###$$#$#$###$##########@##@@####$$$$$$$$$$$$$$$==$==$$$=
==$=$=*=$======$====$=$=$$$##=#$$$$$$$$#$$#######$$#$#$############@@@##$$$#$$$$$$#$$$$$=$==$$===$$$
$$$=====$$==$$======$=$$$$$$#$$$#$#$##$$#$$#######$##############@@@@##$$$#$$$#$$$##$$=$=$=$=$$==$$$

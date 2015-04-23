### [SQF] fn_whoDunnit.sqf
#### Compatibility: 3.x.x & 4.x.x
#### Overrides default death message with a more advanced one.  
  
#####In mpmissions\init.sqf, add:
######fn_whoDunnit = compile preprocessFileLineNumbers "scripts\fn_whoDunnit.sqf";   
  
#####In mpmissions\core\init.sqf, add:  
######player addEventHandler ["Killed", {[player,_this select 1] spawn fn_whoDunnit;}];  
  	
#####Disable deathMessages in Profile Settings for this script to override.  
#include <dpp.a>

var::{variable}<[MAX_PLAYERS]>;

var::{stock script}<=1>;

var::{stock k=1, l = 4, h=9}<+4>;

decl:: Function:{stock main}(args:[])
do..
    Console_Write<string:["GameMode Loaded."]>;
    Console_Write<string:["One:%i",1]>;
done;

decl:: Function:{init}(args:[a,b,c,d])
do..
    Console_Write<string:["%i, %i, %i, %i",a,b,c,d]>;
    return::val<1>;
done;

use:: Callback:{OnGameModeInit}(values:[])
do..
    use:: Function:{init}(args:[234435,234,65,4]);
    return::val<1>;
done;

use:: Callback:{OnPlayerSpawn}(values:[playerid])
do..
    variable[playerid] = 1;
    use:: Function:{SendClientMessage}(args:[playerid, -1, "Welcome"]);
    return:: val<1>;
done;

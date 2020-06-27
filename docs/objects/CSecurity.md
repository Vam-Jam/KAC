# CSecurity@ class

---

## void reloadSecurity()

<br>
<small>Returns: $void </small>

<br>
<br>

## void saveSecurity()

<br>
<small>Returns: $void </small>

<br>
<br>

## void saveWhitelist()

<br>
<small>Returns: $void </small>

<br>
<br>

## void saveBlacklist()

<br>
<small>Returns: $void </small>

<br>
<br>

## void saveIgnorelist()

<br>
<small>Returns: $void </small>

<br>
<br>

## void saveHideNamelist()

<br>
<small>Returns: $void </small>

<br>
<br>

## void saveSeclevs()

<br>
<small>Returns: $void </small>

<br>
<br>

## void printSeclevs()

<br>
<small>Returns: $void </small>

<br>
<br>

## void printPlayerSeclevs()

<br>
<small>Returns: $void </small>

<br>
<br>

## void printBans()

<br>
<small>Returns: $void </small>

<br>
<br>

## void printIgnores()

<br>
<small>Returns: $void </small>

<br>
<br>

## int getSeclevsSize()

<br>
<small>Returns: $int </small>

<br>
<br>

## void emptySeclevs()

<br>
<small>Returns: $void </small>

<br>
<br>

## void sendSeclevs()

<br>
<small>Returns: $void </small>

<br>
<br>

## void sendSeclevs(CPlayer@ player)

<br>
<small>Returns: $void </small>

<br>
<br>

## CSeclev@ getSeclev(const int seclevID)

<br>
<small>Returns: $CSeclev@ </small>

<br>
<br>

## CSeclev@ getSeclev(const string seclevName)

<br>
<small>Returns: $CSeclev@ </small>

<br>
<br>

## void setPlayerSeclev(CPlayer@ player, CSeclev@ seclev)

<br>
<small>Returns: $void </small>

<br>
<br>

## CSeclev@ getPlayerSeclev(CPlayer@ player)

<br>
<small>Returns: $CSeclev@ </small>

<br>
<br>

## CSeclev@ updatePlayerSeclev(CPlayer@ player)

<br>
<small>Returns: $CSeclev@ </small>

<br>
<br>

## bool assignSeclev(CPlayer@ assignerPlayer, CPlayer@ assigneePlayer, CSeclev@ seclev)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool assignSeclev(CPlayer@ player, CSeclev@ seclev)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool checkAccess_Command(CPlayer@ player, const string command)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool checkAccess_Feature(CPlayer@ player, const string feature)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool checkAccess_Assign(CPlayer@ assignerPlayer, CPlayer@ assigneePlayer, CSeclev@ seclev)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool getWhitelistActive()

<br>
<small>Returns: $bool </small>

<br>
<br>

## void ban(CPlayer@ player, const int minutes)

<br>
<small>Returns: $void </small>

<br>
<br>

## void ban(CPlayer@ player, const int minutes, const string reason)

<br>
<small>Returns: $void </small>

<br>
<br>

## void ban(const string username, const int minutes)

<br>
<small>Returns: $void </small>

<br>
<br>

## void ban(const string username, const int minutes, const string reason)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool unBan(const int index)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool unBan(const string username)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void ignore(CPlayer@ player, const int minutes)

<br>
<small>Returns: $void </small>

<br>
<br>

## void ignore(const string username, const int minutes)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool unIgnore(const int index)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool unIgnore(const string username)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void hidename(CPlayer@ player, const int minutes)

<br>
<small>Returns: $void </small>

<br>
<br>

## void hidename(const string username, const int minutes)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool showname(const int index)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool showname(const string username)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool isPlayerBanned(CPlayer@ player)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool isPlayerBanned(const string username)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool isPlayerIgnored(CPlayer@ player)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool isPlayerIgnored(const string username)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool isPlayerNameHidden(CPlayer@ player)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool isPlayerNameHidden(const string username)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void listCheckAllPlayers()

<br>
<small>Returns: $void </small>

<br>
<br>

## void expireBans()

<br>
<small>Returns: $void </small>

<br>
<br>

## void expireIgnores()

<br>
<small>Returns: $void </small>

<br>
<br>

## void expireHideNames()

<br>
<small>Returns: $void </small>

<br>
<br>

## bool bansExist()

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool ignoresExist()

<br>
<small>Returns: $bool </small>

<br>
<br>


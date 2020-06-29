# CBrain@ class

---

## int failtime_end

<br>
<small>Returns: $int </small>

<br>
<br>

## int plannerMaxSteps

<br>
<small>Returns: $int </small>

<br>
<br>

## int plannerSearchSteps

<br>
<small>Returns: $int </small>

<br>
<br>

## int lowLevelSteps

<br>
<small>Returns: $int </small>

<br>
<br>

## int lowLevelMaxSteps

<br>
<small>Returns: $int </small>

<br>
<br>

## CBlob@ getBlob()

<br>
<small>Returns: $CBlob@ </small>

<br>
<br>

## void server_SetActive(bool active)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool isActive()

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool RemoveScript(const string&in fileName)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool AddScript(const string&in fileName)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool hasScript(const string&in fileName)

<br>
<small>Returns: $bool </small>

<br>
<br>

## BrainVars@ getVars()

<br>
<small>Returns: $BrainVars@ </small>

<br>
<br>

## CBlob@ getTarget()

<br>
<small>Returns: $CBlob@ </small>

<br>
<br>

## void SetTarget(CBlob@ blob)

<br>
<small>Returns: $void </small>

<br>
<br>

## void SetPathTo(Vec2f endpoint, bool ignoreGravity)

<br>
<small>Returns: $void </small>

<br>
<br>

## void SetPathTo(Vec2f endpoint, int search_style)

<br>
<small>Returns: $void </small>

<br>
<br>

## Vec2f getPathPosition()

<br>
<small>Returns: $Vec2f </small>

<br>
<br>

## Vec2f getNextPathPosition()

<br>
<small>Returns: $Vec2f </small>

<br>
<br>

## int getPathSize()

<br>
<small>Returns: $int </small>

<br>
<br>

## Vec2f getPathPositionAtIndex(int index)

<br>
<small>Returns: $Vec2f </small>

<br>
<br>

## void SetSuggestedKeys()

<br>
<small>Returns: $void </small>

<br>
<br>

## BrainState getState()

<br>
<small>Returns: $BrainState </small>

<br>
<br>

## string getStateString()

<br>
<small>Returns: $string </small>

<br>
<br>

## bool SetHighLevelPath(Vec2f start, Vec2f end)

<br>
<small>Returns: $bool </small>

<br>
<br>

## int getHighPathSize()

<br>
<small>Returns: $int </small>

<br>
<br>

## Vec2f getHighPathPositionAtIndex(int index)

<br>
<small>Returns: $Vec2f </small>

<br>
<br>

## Vec2f getClosestNodeAtPosition(Vec2f pos)

<br>
<small>Returns: $Vec2f </small>

<br>
<br>

## void SetLowLevelPath(Vec2f start, Vec2f end)

<br>
<small>Returns: $void </small>

<br>
<br>

## void ResetLowLevelPath()

<br>
<small>Returns: $void </small>

<br>
<br>

## void EndPath()

<br>
<small>Returns: $void </small>

<br>
<br>

## Vec2f getShootAimPosition(Vec2f targetPos, bool hardShot, bool&out worthShooting, const float heightModifier)

<br>
<small>Returns: $Vec2f </small>

<br>
<br>

## ScriptData@ getCurrentScript()

<br>
<small>Returns: $ScriptData@ </small>

<br>
<br>

## bool PlanStatePath(PlannerState@ start, PlannerState@ end)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool StatePathStep()

<br>
<small>Returns: $bool </small>

<br>
<br>

## PlannerState@ AddPlannerState(const string&in name)

<br>
<small>Returns: $PlannerState@ </small>

<br>
<br>

## bool getPlannerStates(PlannerState@[]@ states)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool getPlannerSolution(PlannerState@[]@ states)

<br>
<small>Returns: $bool </small>

<br>
<br>

## PlannerState@ getPlannerState(const string&in name)

<br>
<small>Returns: $PlannerState@ </small>

<br>
<br>


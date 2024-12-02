# NFLAFB
**American Football**

**NFL Big Data Bowl 2025 Dataset Summary**
 
Before delving into the NFL dataset, let's first know what we actually mean by the NFL.. Ooops! Before that let me first explain :What is American Football …..?? 

  American Football popularly known as the Rugby football or gridiron Originated in United States. In American Football, each team has 11 players on the field at 
a time, split into different roles depending on whether they're on offense, defense, or special teams. The 
offensive team's goal is to move the ball toward the opponent's end zone to score points, while the 
defense works hard to stop them and take the ball back. Special teams come in for specific situations, 
like kickoffs or field goals. Each player has a unique role: the quarterback leads the offense, calling 
plays and passing the ball; running backs and wide receivers focus on advancing the ball, while linemen 
protect the quarterback and clear the way. On defense, players like linebackers and cornerbacks cover 
the field and stop offensive players from gaining yards. 
The game kicks off with a coin toss, and the winning team decides whether to receive or kick 
the ball. Once the ball is kicked off, the offense has four attempts (or "downs") to gain at least 
10 yards; if they succeed, they get a fresh set of downs to keep advancing toward the end zone. 
If they can’t make it in those four tries, the other team gets the ball. Teams keep switching 
between offense and defense over four quarters, each lasting 15 minutes. When the clock runs 
out, the team with the most points wins the game.  

**What is NFL..?**
The National Football League, or NFL, is currently the top American football league, including 
the top clubs and players in the game. We can examine this game in great detail by analyzing 
NFL data, which includes everything from player statistics and game outcomes to sophisticated 
performance and strategy analytics. Let's examine this dataset and see what the data shows 
about one of the most watched sports in the United States.          
Now coming to the Dataset:   
The Dataset is taken from the kaggle. 

**Dataset Overview**
The dataset for the 2025 Big Data Bowl contains detailed tracking data and additional statistics 
from NFL games. This includes data provided by NFL Next Gen Stats and Pro Football Focus 
(PFF) to give insights into plays, players, and in-game events. Supplemental NFL data from 
public sources like nflverse and Pro Football Reference can also be used.     

**Key Data Files**
Each file provides a different aspect of the game data, covering games, plays, players, and 
player performance: 

➢ **Game Data (games.csv):** This file contains team and game-level details such as 
• gameId: A unique numerical identifier for each game. 
• season: Indicates the season in which the game was played. 
• week: Refers to the specific week of the season. 
• gameDate: The date of the game, formatted as mm/dd/yyyy. 
• gameTimeEastern: The Eastern Standard Time (EST) at which the game  
started in HH:MM format. 
• homeTeamAbbr: A three-letter abbreviation representing the home team. 
• visitorTeamAbbr: A three-letter abbreviation representing the visiting team. 
• homeFinalScore: The total points scored by the home team in the game. 
• visitorFinalScore: The total points scored by the visiting team in the game. 
• The key variable is Gameid in this file. 

➢ **Play Data (plays.csv):** 
• gameId: Unique identifier for each game (numeric). 
• playId: Identifier for each play; not unique across games (numeric). 
• playDescription: Description of the play (text). 
• quarter: Quarter of the game when play occurred (numeric). 
• down: Down for the play (numeric). 
• yardsToGo: Distance required for a first down (numeric). 
• possessionTeam: Abbreviation of the offensive team with possession (text). 
• defensiveTeam: Abbreviation of the team on defense (text). 
• yardlineSide: 3-letter code for the team associated with the line-of-scrimmage 
(text). 

• yardlineNumber: Yard line at line-of-scrimmage (numeric). 
• gameClock: Time on game clock when play occurred (MM). 
• preSnapHomeScore: Home team’s score before the play (numeric). 
• preSnapVisitorScore: Visiting team’s score before the play (numeric). 
• playNullifiedByPenalty: Indicates if the play outcome was nullified due to a 
penalty (Y/N). 
• absoluteYardlineNumber: Distance from the end zone for the team with 
possession (numeric). 
• preSnapHomeTeamWinProbability: Win probability of the home team before 
the play (numeric). 
• preSnapVisitorTeamWinProbability: Win probability of the visiting team 
before the play (numeric). 
• expectedPoints: Expected points on this play (numeric). 
• offenseFormation: Formation used by the team with possession (text). 
• receiverAlignment: Alignment configuration of receivers, specified as 0x0, 
1x0, etc. (text). 
• playClockAtSnap: Value on the play clock at the time of the snap (numeric). 
• passResult: Outcome of the play if a dropback occurred (e.g., Complete, 
Incomplete, Sack, Intercepted, etc.). 
• passLength: Distance the ball traveled beyond the line of scrimmage (LOS); 
negative values if behind LOS (numeric). 
• targetX: X-coordinate of the targeted receiver when the pass arrived (numeric). 
• targetY: Y-coordinate of the targeted receiver when the pass arrived (numeric). 
• playAction: Indicates if there was play-action on the play (Boolean). 
• dropbackType: Type of dropback by the QB after the snap (text). 
• dropbackDistance: Distance QB dropped back behind center (numeric). 
• passLocationType: Location of the QB at the time of throw (text). 
• timeToThrow: Time from snap to pass (in seconds) (numeric). 
• timeInTackleBox: Time QB spent inside the tackle box (numeric). 
• timeToSack: Time from snap to QB being sacked (numeric). 
• passTippedAtLine: Indicates if the pass was tipped at the line of scrimmage 
(Boolean). 
• unblockedPressure: Indicates if there was pressure from an unblocked player 
(Boolean). 
• qbSpike: Indicates if the play was a QB Spike (Boolean). 
• qbKneel: Indicates if the play was a QB Kneel (Boolean). 
• qbSneak: Indicates if the play was a QB Sneak (Boolean). 
• rushLocationType: Direction of the runner based on offensive linemen's 
positioning (text). 
• penaltyYards: Yards gained by offense due to a penalty (numeric). 
• prePenaltyYardsGained: Net yards gained by offense before penalty 
(numeric). 
• yardsGained: Net yards gained by offense including penalty (numeric). 
• homeTeamWinProbabilityAdded: Change in win probability for the home 
team (numeric). 
• visitorTeamWinProbabilityAdded: Change in win probability for the visitor 
team (numeric). 
• expectedPointsAdded: Additional expected points generated by the play 
(numeric). 
• isDropback: Indicates if the play involved a dropback (Boolean). 
• pff_runConceptPrimary: Primary run concept on the play (text). 
• pff_runConceptSecondary: Secondary run concept on the play (text). 
• pff_runPassOption: Indicates if the play was a run-pass option (numeric). 
• pff_passCoverage: Pass coverage concept used by the defense (text). 
• pff_manZone: Type of defense coverage used, man or zone (text). 
➢ Player Data (players.csv):  
• nflId: Unique identification number assigned to each player (numeric). 
• height:Players height (in text format, e.g..”6’2”). 
• weight:Players weight in pounds (numeric). 
• birthDate: Players date of birth (formatted as YYYY-MM-DD). 
• collegeName: Name of the college where the player studied or played (text). 
• position: Official position of the player on the team (text). 
• displayName: Player's full name as displayed (text). 
The Key Varibale is nflId. 

➢ **Player Play Data (player_play.csv)**: Key variables: gameId, playId, nflId.  
• gameId: Unique identifier for each game (numeric). 
•  playId: Identifier for each play, not unique across games (numeric). 
•  nflId: Unique identifier for each player (numeric). 
•  teamAbbr: Abbreviation of the team the player represents (text). 
•  hadRushAttempt: Indicator of whether the player attempted a rush on this 
play (numeric). 
•  rushingYards: Total yards gained from rushing by the player on this play 
(numeric). 
•  hadDropback: Indicator of whether the player dropped back during this play   
(numeric). 
•  passingYards: Total pass yards gained by the player on this play (numeric). 
•  sackYardsOffense: Total yards lost due to a sack for the player on this play  
(numeric). 
•  hadPassReception: Indicator of whether the player caught a pass on this play  
(numeric). 
•  receivingYards: Total receiving yards gained by the player on this play  
(numeric). 
•  wasTargettedReceiver: Indicator of whether the player was the intended  
receiver on this play (numeric). 
•  yardageGainedAfterTheCatch: Yards gained by the player after making the  
catch (numeric). 
•  fumbles: Number of times the player fumbled on this play (numeric). 
•  fumbleLost: Indicator of whether the player lost a fumble to the opposing  
team (numeric). 
•  fumbleOutOfBounds: Indicator of whether the player fumbled out of bounds  
\(numeric). 
•  assistedTackle: Indicator of whether the player assisted in a tackle (numeric). 
•  forcedFumbleAsDefense: Indicator of whether the player forced a fumble by  
the opposing team (numeric). 
•  halfSackYardsAsDefense: Yards lost by offense due to a half-sack by this  
player (numeric). 
•  passDefensed: Indicator of whether a pass was stopped by the player  
(numeric). 
•  quarterbackHit: Indicator of whether the player recorded a QB hit (numeric). 
•  sackYardsAsDefense: Yards lost by the offense due to a sack by this player  
(numeric). 
•  safetyAsDefense: Indicator of whether the player forced a safety (numeric). 
•  soloTackle: Indicator of whether the player made a solo tackle (numeric). 
•  tackleAssist: Indicator of whether the player assisted in a tackle (numeric). 
•  tackleForALoss: Indicator of whether the player tackled behind the line of  
scrimmage (numeric). 
•  tackleForALossYardage: Yards lost by the offense due to a tackle behind the  
line of scrimmage (numeric). 
•  hadInterception: Indicator of whether the player intercepted a pass (numeric). 
•  interceptionYards: Yards returned by the player on an intercepted pass    
(numeric). 
•  fumbleRecoveries: Number of fumbles recovered by the player (numeric). 
•  fumbleRecoveryYards: Yards returned by the player on a fumble recovery  
(numeric). 
•  wasInitialPassRusher: Indicator of whether the player was the initial pass  
rusher (numeric). 
•  penaltyNames: Names of penalties called on this player during this play (text). 
•  causedPressure: Indicates if the player applied pressure on the QB (Boolean). 
•  timeToPressureAsPassRusher: Time from snap to first pressure probability  
of ≥ 0.75 by the player (numeric). 
•  getOffAsPassRusher: Time it took for the player to cross the line of  
scrimmage after the snap (numeric). 
•  inMotionAtBallSnap: Indicates if the player was moving at snap (Boolean). 
•  shiftSinceLineset: Indicates if the player shifted >2.5 yards from the lineset  
position (Boolean). 
•  motionSinceLineset: Indicates if the player moved after initially setting at the  
line (Boolean). 
•  wasRunningRoute: Indicates if the player was running a route (Boolean). 
•  routeRan: The route name the player ran on this play (text). 
•  blockedPlayerNFLId1, 2, 3: NFL IDs of opponents the player blocked on this  
play (numeric). 
•  pressureAllowedAsBlocker: Indicates if any pass rushers matched against this  
player applied pressure (numeric). 
•  timeToPressureAllowedAsBlocker: Time from snap to first instance of ≥  
0.75 pressure probability by a blocked pass rusher (numeric). 
•  pff_defensiveCoverageAssignment: Defensive coverage assignment for the  
player on this play (text). 
• Possible values: MAN, 2R, 2L, 3R, 3M, 3L, 4OR, 4OL, 4IR, 4IL, FR,  FL,  
HCR, HCL, CFR, CFL, HOL, DF, PRE. 
•  pff_primaryDefensiveCoverageMatchupNflId: NFL ID of the primary  
matchup in coverage for the player (numeric). 
•  pff_secondaryDefensiveCoverageMatchupNflId: NFL ID of the secondary      
matchup in coverage for the player (numeric). 
Key Variables for Data Integration 
To merge data across files and external sources, the following key variables are used: 
• gameId: Identifies each game uniquely across all files. 
• playId: Identifies each play within a game (not unique across games). 
• nflId: Identifies each player uniquely across all player data files. 
➢ **Tracking Data (tracking_week_[week].csv):** Need to go through the dataset…… 

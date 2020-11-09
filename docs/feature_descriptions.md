# Features

This markdown document summarizes the three types of features and then provides a list of designed features.

## Regular Features

Regular features are the player averages of scaled raw in-game statistics for each player.

## Ratio Features

Ratio features are the averages of the ratio of a scaled raw in-game statistic over an unscaled raw in-game statistic for each player.

## Strength Features

Strength features are the binomial statistical test values for ratio variables.

## List of Available Features

|   Feature Name    |    Type    |    Numerator    |    Denominator     |
|interceptions_reg  |Regular     | Interceptions| 1|   
|shot_assists_reg   |Regular| Shot Assists| 1|
|key_passes_str     |Strength| Successful Key Passes| Key Passes|
|looseballs_str     |Strength| Looseball Duels Won| Looseball Duels|
|crosses_str        |Strength|Successful Crosses|Crosses|
|long_passes_str    |Strength|Sucessful Long Passes|Long Passes|
|losses_to_recoveries_rat|Ratio|Recoveries|Losses|
|forward_passes_str |Strength|Successful Fwd Passes| Forward Passes|
| passes_str        |Strength|Successful Passes|Passes|
|through_passes_str |Strength|Successful Through Passes|Through Passes|
|passes_to_final_third_str|Strength|Successful Passes to Final Third| Passes to Final Third|
|linkup_plays_str   |Strength|Successful Linkup Plays|Linkup Plays|
|accelerations_reg  |Regular|Accelerations| 1|
|fouls_reg          |Regular|Fouls| 1|
|xgshots_reg        |Regular|xgShot| 1|
|xgassists_reg      |Regular|xgAssist| 1|
|successful_dribbles_str|Strength|Successful Dribbles|Dribbles
|progressive_runs_reg|Regular|Progressive Runs| 1 |
|pressing_duels_reg |Regular|Pressing Duels| 1|
|received_passes_reg|Regular|Received Passes| 1|
|forward_to_back_and_vert_passes_rat|Ratio|Forward Passes| Vertical Passes + Back Passes|
|field_air_duels_str|Strength|Field Aerial Duels Won|Field Aerial Duels|
|opponent_half_recoveries_reg|Regular|Opponent Half Recoveries|1|
|recoveries_to_fouls_rat|Ratio|Recoveries|Fouls|
|shots_reg|Regular|Shots|1|
|defensive_duels_str|Strength|Defensive Duels Won|Defensive Duels|
|attacking_duels_str|Strength|Offensive Duels Won|Offensive Duels|
|own_half_losses_reg|Regular|Own Half Losses|1|
|net_expected_goals|Regular|Goals - Xgshot|1|
|shots_str|Strength|Shots on Target|Shots|1|
|headshots_reg|Regular|Head Shots|1|

# A ML approach to predicting the valuations of football players

## Student Info

**School**: University of the West of England, Bristol, England, UK.  
**Student ID**: 22037705  
**Programme**: M.Sc. Data Science 2022/2023 session

## FIFA Dataset columns and used status

| Column Name                 | Column Description | Is Column Used |
| --------------------------- | ------------------ | -------------- |
| sofifa_id                   | ---                | no             |
| player_url                  | ---                | no             |
| short_name                  | ---                | no             |
| long_name                   | ---                | no             |
| player_positions            | ---                | yes            |
| overall                     | ---                | yes            |
| potential                   | ---                | yes            |
| value_eur                   | ---                | yes            |
| wage_eur                    | ---                | yes            |
| age                         | ---                | yes            |
| dob                         | ---                | no             |
| height_cm                   | ---                | yes            |
| weight_kg                   | ---                | yes            |
| club_team_id                | ---                | no             |
| club_name                   | ---                | yes            |
| league_name                 | ---                | yes            |
| league_level                | ---                | no             |
| club_position               | ---                | no             |
| club_jersey_number          | ---                | no             |
| club_loaned_from            | ---                | no             |
| club_joined                 | ---                | no             |
| club_contract_valid_until   | ---                | yes            |
| nationality_id              | ---                | no             |
| nationality_name            | ---                | yes            |
| nation_team_id              | ---                | no             |
| nation_position             | ---                | no             |
| nation_jersey_number        | ---                | no             |
| preferred_foot              | ---                | yes            |
| weak_foot                   | ---                | yes            |
| skill_moves                 | ---                | yes            |
| international_reputation    | ---                | yes            |
| work_rate                   | ---                | yes            |
| body_type                   | ---                | no             |
| real_face                   | ---                | no             |
| release_clause_eur          | ---                | no             |
| player_tags                 | ---                | no             |
| player_traits               | ---                | no             |
| pace                        | ---                | yes            |
| shooting                    | ---                | yes            |
| passing                     | ---                | yes            |
| dribbling                   | ---                | yes            |
| defending                   | ---                | yes            |
| physic                      | ---                | yes            |
| attacking_crossing          | ---                | yes            |
| attacking_finishing         | ---                | yes            |
| attacking_heading_accuracy  | ---                | yes            |
| attacking_short_passing     | ---                | yes            |
| attacking_volleys           | ---                | yes            |
| skill_dribbling             | ---                | yes            |
| skill_curve                 | ---                | yes            |
| skill_fk_accuracy           | ---                | yes            |
| skill_long_passing          | ---                | yes            |
| skill_ball_control          | ---                | yes            |
| movement_acceleration       | ---                | yes            |
| movement_sprint_speed       | ---                | yes            |
| movement_agility            | ---                | yes            |
| movement_reactions          | ---                | yes            |
| movement_balance            | ---                | yes            |
| power_shot_power            | ---                | yes            |
| power_jumping               | ---                | yes            |
| power_stamina               | ---                | yes            |
| power_strength              | ---                | yes            |
| power_long_shots            | ---                | yes            |
| mentality_aggression        | ---                | yes            |
| mentality_interceptions     | ---                | yes            |
| mentality_positioning       | ---                | yes            |
| mentality_vision            | ---                | yes            |
| mentality_penalties         | ---                | yes            |
| mentality_composure         | ---                | yes            |
| defending_marking_awareness | ---                | yes            |
| defending_standing_tackle   | ---                | yes            |
| defending_sliding_tackle    | ---                | yes            |
| goalkeeping_diving          | ---                | no             |
| goalkeeping_handling        | ---                | no             |
| goalkeeping_kicking         | ---                | no             |
| goalkeeping_positioning     | ---                | no             |
| goalkeeping_reflexes        | ---                | no             |
| goalkeeping_speed           | ---                | no             |
| ls                          | ---                | no             |
| st                          | ---                | no             |
| rs                          | ---                | no             |
| lw                          | ---                | no             |
| lf                          | ---                | no             |
| cf                          | ---                | no             |
| rf                          | ---                | no             |
| rw                          | ---                | no             |
| lam                         | ---                | no             |
| cam                         | ---                | no             |
| ram                         | ---                | no             |
| lm                          | ---                | no             |
| lcm                         | ---                | no             |
| cm                          | ---                | no             |
| rcm                         | ---                | no             |
| rm                          | ---                | no             |
| lwb                         | ---                | no             |
| ldm                         | ---                | no             |
| cdm                         | ---                | no             |
| rdm                         | ---                | no             |
| rwb                         | ---                | no             |
| lb                          | ---                | no             |
| lcb                         | ---                | no             |
| cb                          | ---                | no             |
| rcb                         | ---                | no             |
| rb                          | ---                | no             |
| gk                          | ---                | no             |
| player_face_url             | ---                | no             |
| club_logo_url               | ---                | no             |
| club_flag_url               | ---                | no             |
| nation_logo_url             | ---                | no             |
| nation_flag_url             | ---                | no             |

## Data Cleaning and Preprocessing

1. Remove unused columns.
2. Rename `player_positions` column to `position` and update values to _defender_, _midfielder_, and _forward_ based on value.
3. Remove rows with missing/null values.

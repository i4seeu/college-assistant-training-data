## happy path
* greet
  - utter_greet
* mood_great
  - utter_happy

## sad path 1
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* deny
  - utter_goodbye

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot
## fees greet path
* greet
  - utter_need_help
* school_fees
  - utter_category
* indicate_category
  - action_retrieve_fees
* mood_great
  - utter_goodbye
## fees together with category
* school_fees{"student_category":"local"}
  - action_retrieve_fees
* mood_great
  - utter_goodbye
## fees greet path
* school_fees
  - utter_category
* indicate_category
  - action_retrieve_fees
* mood_great
  - utter_goodbye


## programme greet path
* greet
  - utter_need_help
* programmes
  - utter_level
* indicate_level
  - action_retrieve_programmes
* mood_great
  - utter_goodbye

## programme together with level path
* programmes {"programme_level":"undergraduate"}
  - action_retrieve_programmes
* mood_great
  - utter_goodbye

## programme greet path
* programmes
  - utter_level
* indicate_level
  - action_retrieve_programmes
* mood_great
  - utter_goodbye


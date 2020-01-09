## happy path
* greet
  - utter_greet
  - utter_name
* mood_great
  - utter_happy
  
 ## sad path 1
* greet
  - utter_greet
  - utter_name
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
  - utter_name
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* deny
  - utter_goodbye
  
## Generated Story -250213808576262513
* greet
    - utter_greet
    - utter_name
* name
    - utter_utilities
* task
    - utter_task
* position
    - utter_role
* position{"role_type": "technical"}
    - slot{"role_type": "technical"}
    - action_check_positions
    - slot{"positions": ["machine learning engineer", "ML product success engineer"]}
    - utter_email
* give_email
    - utter_mobile
* give_tel
    - utter_goodbye
    
## Generated Story -250213808576262514
* greet
    - utter_greet
    - utter_name
* name
    - utter_utilities
* position
    - utter_role
* position{"role_type": "technical"}
    - slot{"role_type": "technical"}
    - action_check_positions
    - slot{"positions": ["machine learning engineer", "ML product success engineer"]}
    - utter_email
* give_email
    - utter_mobile
* give_tel
    - utter_goodbye
    

## Generated Story 2565143873267614185
* greet
    - utter_greet
    - utter_name
* name
    - utter_utilities
* position
    - utter_role
* position{"role_type": "any"}
    - slot{"role_type": "any"}
    - action_check_positions
    - slot{"positions": ["machine learning engineer", "ML product success engineer"]}
    - utter_goodbye


## Generated Story -250213808576262516
* greet
    - utter_greet
    - utter_name
* name
    - utter_utilities
* position
    - utter_role
* position{"role_type": "business"}
    - slot{"role_type": "business"}
    - action_check_positions
    - slot{"positions": []}
    - utter_email
* give_email
    - utter_mobile
* give_tel
    - utter_getback

## Generated Story -250213808576262518
* greet
    - utter_greet
    - utter_name
* name
    - utter_utilities
* task
    - utter_task
* position
    - utter_role
* position{"role_type": "business"}
    - slot{"role_type": "business"}
    - action_check_positions
    - slot{"positions": []}
    - utter_getback
    
## Generated Story -250213808576262519
* greet
    - utter_greet
    - utter_name
* name
    - utter_utilities
* position
    - utter_role
* position{"role_type": "business"}
    - slot{"role_type": "business"}
    - action_check_positions
    - slot{"positions": ["BD"]}
    - utter_email
* give_email
    - utter_mobile
* give_tel
    - utter_getback
    
## Generated Story -4339520876749317291
* greet+position
    - utter_simple_greet
    - utter_role
* position{"role_type": "technical"}
    - slot{"role_type": "technical"}
    - action_check_positions
    - slot{"positions": ["machine learning engineer", "ML product success engineer"]}
    - utter_email
* give_email
    - utter_mobile
* give_tel
    - utter_goodbye
    
## Generated Story -4339520876749317292
* greet+position
    - utter_simple_greet
    - utter_role
* position{"role_type": "business"}
    - slot{"role_type": "business"}
    - action_check_positions
    - slot{"positions": []}
    - utter_email
* give_email
    - utter_mobile
* give_tel
    - utter_getback
    
## Thank Story
* thanks
    - utter_nothanks
    
## Bye Story
* goodbye
    - utter_goodbye
<!--para cada título, um caminho. exemplo abaixo: -->
## happy path 
<!--Caminho oi, tudo bem, como vc esta? estou feliz? -->
* greet
<!--o greet acima até em nlu.md, se der match nele, chama o utter_greet abaixo, que esta em domain.yml-->
  - utter_greet
* mood_great
<!--mood_great esta em nlu.md e se refere às possíveis respostas positivas do usuário. Se der match, chama utter_happy, que esta em domain.yml-->
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

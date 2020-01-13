# RASA_Chatbot
Sample chatbot created using RASA_core, rasa_NLU and RasaX.

#### Rasa is a set of open source machine learning tools for developers for conversational AI.

#### NLU : an open source natural language processing tool for intent classification and entity extraction.

#### Intent – lebels, user input overall meaning category.

#### Entity – information that can extract from the input. (Uses name entity model which helps to extract from the user input).

#### RASA NLU(component) – enables the assistance to understand what the user said.
#### RASA Core(Dialogue management component) – Makes predictions how the assistance should respond.
#### RASA X – Enables to assistance to continue learning from the real time data.

## RASA Installation Guide:

-  Spacy : *pip install -U spacy*

-  Spacy Large English language model : *python -m spacy download en_core_web_sm*

-  Link the model now: *python -m spacy link en_core_web_sm en*

-  RASA X installation : *pip install rasa-x --extra-index-url https://pypi.rasa.com/simple*

For step by step procedure to create and run a Rasa project follow the tutorial:
https://rasa.com/docs/rasa/user-guide/rasa-tutorial/

# Rasa Chatbot Components:

## RASA NLU:(nlu.md)
Rasa should understand user messages, and then train a model by showing it those examples.
"## intent: <intent name>"

## RASA stories:(stories.md)
User inputs express in intents and entity
'##' -  name of the story
‘*’ – messages input by users, entity we can provide using {}
‘-‘ – starts with ‘-‘. Two types of actions 1. Utterances 2. And custom actions.

## RASA Domains:(domain.yml)
A domain is very important part and defines the universe in which assistance operates.
‘domain.yml’
1.	intents – list of intents the assistance understand.
2.	Entities -  how the user data.
3.	Actions – list of all utterances and custom actions an assistance should use to response.
4.	Templates – Actually responses the assistance gives to the user.

## Configuration File:(config.yml)
The configuration file defines the NLU and Core components that your model will use. In this example, your NLU model will use the supervised_embeddings pipeline. You can learn about the different NLU pipelines here.

# Train Rasa Model:
Anytime we add new NLU or Core data, or update the domain or configuration, we need to re-train a neural network on our example stories and NLU data. To do this, run the command below. This command will call the Rasa Core and NLU train functions and store the trained model into the models/ directory. The command will automatically only retrain the different model parts if something has changed in their data or configuration.

*rasa train* - Train both rasa core and rasa nlu
*rasa train nlu* - train onlu rasa nlu

# Talk to your assitance:
We can talk to the trained assitance in command promt or can connect to any UI.

To run in command promt:

*rasa shell*

**note: *rasa shell nlu* - It show how your bot understands the user inputs.**

**note: *rasa visualize* - Creates a graph of the conversation flow.**

**note: *rasa x* - opens up a GUI platform for deveoplment of the Rasa bot**

# Run Chatbot from UI(webchat):

- add below text in *credentials.yml* file.

**socketio:
  user_message_evt: user_uttered
  bot_message_evt: bot_uttered
  session_persistence: true**
  
- Use the below script file in your webpage:

<div id="webchat"/>
  <script src="static/js/webchat-v0.7.8.js"></script>
  <script>
    WebChat.default.init({
      selector: "#webchat",
      interval: 1000, // 1000 ms between each message
      customData: {"userId": "123"}, // arbitrary custom data. Stay minimal as this will be added to the socket
      socketUrl: "http://localhost:5005",
      socketPath: "/socket.io/",
      title: "Rasa Bot",
      subtitle: "AI powered Conversational Bot",
      inputTextFieldHint: "Type a message...",
      connectingText: "Waiting for server...",
      hideWhenNotConnected: true,
      fullScreenMode: false,
      profileAvatar: "static/icons/bot_open.png",
      openLauncherImage: 'static/icons/bot_open.png',
      closeLauncherImage: 'myCustomCloseImage.png',
      params: {
        images: {
          dims: {
            width: 600,
            height: 600,
          }
        },
        storage: "local"
      }
    })
  </script>





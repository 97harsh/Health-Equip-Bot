# Health-Equip-Bot
HealthBotEquip: a chatbot for personalized medical equipment recommendations, built with Rasa and Django, and deployed on Kubernetes.

HealthBotEquip is a chatbot that helps healthcare professionals and patients to find the appropriate medical equipment for their needs. The chatbot uses natural language processing (NLP) to understand the user's requirements and provides personalized recommendations for medical equipment, such as wheelchairs, walkers, and other assistive devices. The recommendations are based on the user's inputs, such as medical condition, budget, and other preferences.


HealthBotEquip is built using Rasa, an open-source machine learning framework for building conversational AI, and Django, a high-level Python web framework that enables rapid development and clean design. The chatbot is containerized and deployed on a Kubernetes cluster, which allows for easy scaling and management.


The goal of HealthBotEquip is to simplify the process of finding medical equipment and improve the overall healthcare experience for patients and healthcare professionals. By leveraging the power of AI and machine learning, HealthBotEquip aims to provide personalized and accurate recommendations that meet the unique needs of each user.


### How to install
```
pip install rasa
pip install rasa[transformer]
pip install transformers
python -m spacy download en_core_web_md
```

### Working with the chatbot
To start the chatbot using the command line
```
rasa shell
```

To test the NLU components
```
rasa shell nlu
```

If you're going to use stories which has asociated actions, don't forget to start the server
```
rasa run actions
```

To test if all your YAML files are in correct format you can:
```
rasa data validate
```

To test sample stories are corret:
```
rasa test
```
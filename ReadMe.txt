For this version of Rasa:
Need Python version 3.8 or below and 3.2 and higher.

A major functionality I couldn't manage to make work was getting to put any city and restaurant in the sentence and get it as an entity. 
- I tried creating a list such as cities.yml
- I tried using the entities keyword under the intent in stories.yml
	- But this only worked for the cities or restaurants in the examples of NLU

For that reason this only works with
cities:

denver
chicago
phoenix
washington
las vegas

restaurants:

kfc
subway
mcdonalds

So for running this just run with the following example.
The Spelling mistake functionality does get picked up for the cities if the cities spelling are close e.g: chicago -> chicgo etc.
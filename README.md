# Rasa Bot
## USA Restaurant Recommender


### Set Up


1. Install Rasa
    - Use Python > 3.9 or < 3.1
```shell
virtualenv rasaEnv
python -m pip uninstall pip
python -m ensurepip
python =m pip install -U pip
pip install rasa
```
2. Install other dependencies
```shell
pip install -r requirements.txt
```
3. Run Actions Server
```shell
rasa run actions
```
4. Train Model
```shell
rasa train
```

5. Load and Run Trained Model
```shell
rasa shell
```

6. Create a new basic bot
```shell
rasa init
```

### Note
 
> A major functionality I couldn't manage to make work was getting to put
> any city and restaurant in the sentence and get it as an entity.
> I tried creating a list such as cities.yml
> I tried using the entities keyword under the intent in stories.yml
> But this only worked for the cities or restaurants in the examples of NLU

For that reason this only works with

## Use These Examples

| Cities | Restaurants |
| ------ | ------ |
| denver | kfc |
| chicago | subway |
| phoenix | mcdonalds |
| washington | - |
| las vegas | - |

So for running this just run with the following example.
The Spelling mistake functionality does get picked up for the cities if the cities spelling are close e.g: chicago -> chicgo etc.


### Examples
![Results](Snapshot/Example_Flow_1.PNG)
![Results](Snapshot/Example_Flow_2.PNG)
![Results](Snapshot/Spelling_Mistake.PNG)
![Results](Snapshot/Not_Get_Started.PNG)
![Results](Snapshot/Not_In_List.PNG)



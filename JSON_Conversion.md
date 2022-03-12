# JSON
## Structure faction
````json
{
    "name": "",
    "id": "",
    "author": "",
    "color": "",
    "background": "",
    "strength": "",
    "weaknesses": "",
    "units": {},
    "models": {},
    "weapons": {},
    "rules": {},
    "hidden_relics": {},
    "relics": {},
    "strategies": {},
    "powers": {},
    "powerCategories": {}
}
````
**name**
> Nom de votre faction

**id**
> Identifiant de votre faction doit être unique et sans majuscule, ni espace, ni caractère spécial

**author**
> Auteur de la faction 

**color**
> Couleur de la faction en HEX exemple : #000000

**background**
> Le lore de votre faction

**strenghts**
> Les forces de votre faction

**weaknesses**
> Les faiblesses de votre faction
### Structure Units
````json
"identifiant_de_votre_unite":{
    "name":"",
    "description":"",
    "category":"",
    "keywords":[],
    "rules":[],
    "subfactions":[],
    "models":[]
}
````
Premièrement donner un identifiant a votre unité qui doit être unique et sans majuscule, ni espace, ni caractère spécial

**name**
> Le nom de l'unité

**description**
> La description de l'unité

**category**
> La catégory de l'unité à choix entre *command*, *core*, *specialist*, *strike*, *heavy*, *transport*, *super_heavy*, *fortification*, *flyers*

**keywords**
> Les mots clé de l'unité notés en liste exemple : 
> ````json 
> ["keyword1","keyword2"] 
> ````

**rules**
> Les règles de l'unité notés en liste exemple : 
> ````json 
> ["rule1","rule2"] 
> ````
> Ces règles doivent être des identifiants existants dans les règles de faction

**subfactions**
> Les sous-factions de l'unité notés en liste exemple : 
> ````json 
> ["subfaction1","subfaction2"] 
> ````
> Ces sous-factions doivent être des identifiants existants dans le fichier index.json

**models**
> La liste des models composants l'unité.
> ````json
> {
>    "name": "nom du model",
>    "movement": statistique de mouvement,
>    "courage": statistique de courage,
>    "shoot": statistique de tir,
>    "fight": statistique de corps à corps,
>    "defense": statistique de défense,
>    "reflexes": statistique de réflexes,
>    "thoughness": statistique d'endurance,
>    "attack": statistique du nombre d'attaque,
>    "strength": statistique de force,
>    "points": coup en points par modèle,
>    "wounds": statistique de points de vie,
>    "weapons": [],
>    "options": [
>        {
>            "modelLimit": null,
>            "replaceWeapon": "",
>            "withWeapon": []
>        }
>    ],
>    "rules": [],
>    "min": 4,
>    "max": 9
> }
> ````
> **weapons**
>> liste des armes par défaut de l'unité
>
> **options**
>> Les changements d'armes avec le nombre de modèle pouvant prendre l'arme et qu'est-ce qui remplace ou non ainsi que son coût en points.
>
> **rules**
>> liste des armes par défaut de l'unité
>
> **min**
>> liste des armes par défaut de l'unité
>
> **max**
>> liste des armes par défaut de l'unité
>

### Structure Weapons
### Structure Rules
### Structure Hidden relic
### Structure Relics
### Structure Strategies
### Structure powers
### Structure power Categories

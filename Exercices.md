# Exercices

## Partie 1 : APIs

## Partie 2 : IA

Pour les exercices suivants, partir de la colonne qui contient les données "Présentation du producteur" extraites
à partir des pages de la Bibliothèque de Genève lors de la première partie.

À défaut, importer les données du fichier (data/archives-privees-bibliotheque-de-geneve-enrichies.csv)[`archives-privees-bibliotheque-de-geneve-enrichies.csv`]
dans un nouveau projet OpenRefine et utiliser la colonne `PresentationProducteur`.

### Ajouter un modèle d'IA à OpenRefine

* Vérifier que l'extension [AI Extension for OpenRefine](https://github.com/sunilnatraj/llm-extension) est bien installée
* Ajouter au moins un modèle à choix, soit via une API externe, soit via l'API interne d'Ollama.

<details>
  <summary>Voir quelques exemples de configuration...</summary>
  
  Mistral via l'API d'Infomaniak:
  
  ![Comment configurer l'IA d'Infomaniak dans l'extension OpenRefine](img/settings-infomaniak.png)
  
  Ollama en local:
  
  ![Comment configurer Ollama dans l'extension OpenRefine](img/settings-ollama-local.png)
  
  Pour voir la liste des modèles disponibles, taper `ollama list` dans un terminal. Pour installer un nouveau modèle, il suffit de le lancer avec p.ex. `ollama run llama3.2`. Cela donne quelque chose comme
  
  ```
  NAME                  ID              SIZE      MODIFIED    
  deepseek-r1:latest    6995872bfe4c    5.2 GB    3 weeks ago    
  deepseek-r1:8b        6995872bfe4c    5.2 GB    3 weeks ago    
  llama3.2:latest       a80c4f17acd5    2.0 GB    3 weeks ago
  ```
  
  Utilisez le nom du modèle tel qu'affiché dans la première colonne dans le menu de configuration.
  
  Noter que le bouton "Test service" ne fonctionne souvent pas!
</details>
# French CEDICT · dictionnaire chinois–français ouvert

**124 057 articles téléchargeables : 58 130 traductions CFDICT conservées et 65 927 traductions supplémentaires ayant fait l’objet d’une relecture indépendante par IA.** Ce dépôt communautaire est préparé par le projet [Laowai](https://laowaiapp.com/). Il n’est pas le dépôt officiel de CFDICT et ne revendique aucune approbation de ses mainteneurs.

## Téléchargements

- [Dictionnaire JSON.gz](data/dictionary.json.gz) — texte et provenance par article, statut de relecture et empreintes.
- [Dictionnaire CSV.gz](data/dictionary.csv.gz) — format tabulaire pour consultation et import.
- [Nouveaux articles relus : JSON.gz](data/reviewed-additions.json.gz) et [XML.gz](data/reviewed-additions.xml.gz) — uniquement les 65 927 ajouts, pour proposition aux projets amont.
- [Manifest et SHA-256](data/manifest.json), [source CC-CEDICT exacte](sources/source-records.json.gz), [proposition destinée à CFDICT](UPSTREAM_PROPOSAL.fr.md).

Les traductions sont attachées à l’article entier. Elles ne sont **pas** présentées comme des segments alignés un à un avec chaque sens anglais. Le JSON conserve les segments anglais séparément et utilise `translation_alignment: whole_record`. Le CSV et le XML sont des projections du même texte vérifié, sans réécriture des traductions.

## Origine et méthode

Les caractères traditionnels et simplifiés, le pinyin numéroté et les sens anglais sont appariés à la source publique CC-CEDICT du 23 octobre 2026, conservée à l’identique dans le dépôt chinois–ukrainien, commit `9a2dadcc62bc5a1dec6cf5c84e242c6702f036eb`. Les identités conservent la casse du pinyin. Aucun ID interne d’application, progression, liste HSK, exemple, média ou donnée utilisateur n’est publié.

Les nouveaux textes français ont été rédigés avec **GPT-6.1 Terra, effort xhigh**, puis relus par un autre agent sur le mot chinois, la lecture, la glose anglaise complète et la proposition française. Les rectifications finales effectuées par l’agent principal sont indiquées dans les métadonnées. Des erreurs concrètes et des incertitudes du texte source restent explicitement signalées. Les modèles déclarés ne constituent pas une attestation indépendante du système ayant exécuté les modèles.

Le constructeur a vérifié les vrais dossiers de preuve liés aux sources, aux brouillons et aux verdicts finaux avant cette projection publique. Chaque nouvelle traduction conserve le SHA-256 du texte relu et du document de verdict original. Le validateur public rejoue l’identité de source, les empreintes, les décomptes et l’égalité JSON/CSV/XML. Il ne réexécute pas la relecture linguistique et ne peut pas prouver l’identité de son auteur.

Les 58 130 textes CFDICT conservés ne sont **pas** étiquetés comme nouvellement relus par IA. Leurs sources et leur licence d’origine sont séparées de celles des ajouts. Les sens anglais courants sont fournis comme référence et ne prouvent pas à eux seuls qu’une ancienne définition CFDICT couvre tous leurs sens.

**Aucune validation humaine nouvelle ni mesure de précision globale n’est revendiquée.** `human_validation` et `runtime_approved` restent `false`. Les textes litigieux ou sans correspondance publique exacte sont exclus de cette publication ; ce téléchargement ne prétend pas couvrir toutes les entrées de CC-CEDICT ou terminer la localisation de l’application.

## Vérification

```sh
python3 -B scripts/validate.py
```

Le validateur ne nécessite ni application, ni serveur, ni clé API. Les propositions, réserves et corrections sont bienvenues par issue ou pull request. Citez l’ID public, le chinois, le pinyin exact, le texte français et une source ; distinguez correction de traduction et correction du dictionnaire source.

## Sources et licences

- [CC-CEDICT](https://www.mdbg.net/chinese/dictionary?page=cc-cedict) : CC BY-SA 4.0 ; contributeurs de CC-CEDICT, publication MDBG, projet fondé par Paul Andrew Denisowski.
- [CFDICT / Chine Informations](https://chine.in/mandarin/dictionnaire/CFDICT/) : textes français d’origine, CC BY-SA 3.0 ; contributeurs de CFDICT et Chine Informations, projet créé par David Houstin. Leurs notices et champs de provenance sont conservés.
- Adaptations françaises supplémentaires et cette compilation : **CC BY-SA 4.0**, avec attribution à Laowai et aux sources indiquées. La licence d’origine des contenus conservés n’est pas effacée. [Compatibilité des licences ShareAlike](https://creativecommons.org/compatible-licenses/).
- Le script de validation original de ce dépôt est fourni sous licence MIT, voir `scripts/LICENSE`.

Le dépôt public ne remplace aucune version de CFDICT ou de CC-CEDICT. Une proposition en amont n’est pas une acceptation par ses mainteneurs.

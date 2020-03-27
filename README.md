Traduit de l'original [MMM-TPLink](https://github.com/slametps/MMM-TPLink).

Merci a [Slametps](https://github.com/slametps) pour son travail.

# MMM-TPLink [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)]

Module TPLink Smarthome pour MagicMirror<sup>2</sup>.
Ce module s'inspire et utilise quelques codes de [MMM-Hue](https://github.com/MitchSS/MMM-Hue).

## Materiel supporté

| Modèle                                    | Type |
|------------------------------------------|------|
| HS100, HS105, HS110, HS200               | Plug |
| LB100, LB110, LB120, LB130, LB200, LB230 | Bulb |

## Exemple

![](others/MMM-TPLink-screenshot-01.png)   ![](others/MMM-TPLink-screenshot-02.png)

## Dependances

* Une installation de [MagicMirror<sup>2</sup>](https://github.com/MichMich/MagicMirror).
* [tplink-smarthome-api](https://github.com/plasticrake/tplink-smarthome-api) nodejs module.

## Installation

1. Clone this repo into `~/MagicMirror/modules` directory.
2. Aller dans le repertoire `~/MagicMirror/modules/MMM-TPLink` et lancer `npm install`
3. Ajouter et configurer le module dans le fichier  `~/MagicMirror/config/config.js`:

    ```
    {
        module: 'MMM-TPLink',
        position: 'top_right',
        config: {
        }
    }
    ```

## Options de configuration

| **Option** | **Defaut** | **Description** |
| --- | --- | --- |
| `colour` | `false` | Affichage de l'état de l'alimentation en couleur ou non |
| `updateInterval` | `600000 ms` (10 minutes) | Intervale de mise à jour |
| `showOnlyOn` | `false` | S'il est défini sur true, le module affiche uniquement les voyants allumés |
| `showLabel` | `true` | Afficher l'étiquette d'en-tête ? |
| `timeout` | `3000` | Combien de temps doit prendre la découverte  |
| `animationSpeed` | `2500 ms` (2.5 s) | Vitesse de l'animation de mise à jour |

# Burundi Data for Developers

This repository contains comprehensive data about Burundi in JSON format, designed for developers building applications related to Burundi.

## Overview

The `data.json` file contains structured information about Burundi's administrative divisions, demographics, geography, economy, education, holidays, and more. This data is particularly useful for:

- Building location-based applications
- Creating administrative forms and dropdowns
- Developing educational or informational platforms
- Building maps and geographic applications
- Creating cultural or tourism applications

## Data Structure

### Administrative Divisions

- **Current Provinces (5)**: Buhumuza, Bujumbura, Burunga, Butanyerera, Gitega
- **Old Provinces (18)**: Historical administrative divisions from 2015-2025
- **Communes (42)**: Current administrative subdivisions within provinces
- **Territorial Correspondence**: Mapping between current and former provinces

### Key Data Sections

- **Demographics**: Population statistics, literacy rates, life expectancy
- **Geography**: Area, borders, highest point, major lake, climate
- **Economy**: Currency, GDP growth, major industries, natural resources
- **Education**: School structure, academic calendar, literacy information
- **Holidays**: National and religious holidays with dates
- **Contact Formats**: Phone codes, postal codes, address formats
- **Languages**: Official and local languages
- **Timezones**: Africa/Bujumbura and Central Africa Time (CAT)

### Multilingual Support

The data includes both English and French translations for:

- Province descriptions
- Major industries
- Key attractions
- Climate descriptions
- Holiday names
- Geography information
- Education structure

## Usage Examples

### Get All Provinces

```javascript
const provinces = data.provinces.map((province) => ({
  name: province.name,
  capital: province.capital,
  population: province.population,
}));
```

### Get Communes by Province

```javascript
const bujumburaCommunes = data.provinces.find((p) => p.name === "Bujumbura").communes.map((commune) => commune.name);
```

### Get Holiday Information

```javascript
const holidays = data.holidays.map((holiday) => ({
  date: holiday.date,
  name: holiday.name,
  nameFr: holiday.name_fr,
  type: holiday.type,
}));
```

## Data Updates

This data reflects Burundi's administrative reorganization in 2025, where 18 former provinces were consolidated into 5 current provinces. The territorial correspondence mapping shows how the old provinces were merged.

## Contributing

If you find any inaccuracies or have suggestions for additional data, please feel free to contribute to this repository.

## License

This data is provided for educational and development purposes. Please verify critical information for official use cases.

---

# Données du Burundi pour les Développeurs

Ce repositoire contient des données complètes sur le Burundi au format JSON, conçues pour les développeurs créant des applications liées au Burundi.

## Aperçu

Le fichier `data.json` contient des informations structurées sur les divisions administratives du Burundi, la démographie, la géographie, l'économie, l'éducation, les jours fériés, et plus encore. Ces données sont particulièrement utiles pour :

- Construire des applications basées sur la localisation
- Créer des formulaires administratifs et des listes déroulantes
- Développer des plateformes éducatives ou informatives
- Construire des applications cartographiques et géographiques
- Créer des applications culturelles ou touristiques

## Structure des Données

### Divisions Administratives

- **Provinces Actuelles (5)** : Buhumuza, Bujumbura, Burunga, Butanyerera, Gitega
- **Anciennes Provinces (18)** : Divisions administratives historiques de 2015-2025
- **Communes (42)** : Subdivisions administratives actuelles dans les provinces
- **Correspondance Territoriale** : Cartographie entre les provinces actuelles et anciennes

### Sections Clés des Données

- **Démographie** : Statistiques de population, taux d'alphabétisation, espérance de vie
- **Géographie** : Superficie, frontières, point culminant, lac principal, climat
- **Économie** : Devise, croissance du PIB, industries majeures, ressources naturelles
- **Éducation** : Structure scolaire, calendrier académique, informations sur l'alphabétisation
- **Jours Fériés** : Jours fériés nationaux et religieux avec dates
- **Formats de Contact** : Codes téléphoniques, codes postaux, formats d'adresse
- **Langues** : Langues officielles et locales
- **Fuseaux Horaires** : Africa/Bujumbura et Heure d'Afrique Centrale (CAT)

### Support Multilingue

Les données incluent des traductions en anglais et en français pour :

- Descriptions des provinces
- Industries majeures
- Attractions principales
- Descriptions du climat
- Noms des jours fériés
- Informations géographiques
- Structure éducative

## Exemples d'Utilisation

### Obtenir Toutes les Provinces

```javascript
const provinces = data.provinces.map((province) => ({
  name: province.name,
  capital: province.capital,
  population: province.population,
}));
```

### Obtenir les Communes par Province

```javascript
const communesBujumbura = data.provinces.find((p) => p.name === "Bujumbura").communes.map((commune) => commune.name);
```

### Obtenir les Informations sur les Jours Fériés

```javascript
const holidays = data.holidays.map((holiday) => ({
  date: holiday.date,
  name: holiday.name,
  nameFr: holiday.name_fr,
  type: holiday.type,
}));
```

## Mises à Jour des Données

Ces données reflètent la réorganisation administrative du Burundi en 2025, où 18 anciennes provinces ont été consolidées en 5 provinces actuelles. La cartographie de correspondance territoriale montre comment les anciennes provinces ont été fusionnées.

## Contribution

Si vous trouvez des inexactitudes ou avez des suggestions pour des données supplémentaires, n'hésitez pas à contribuer à ce dépôt.

## Licence

Ces données sont fournies à des fins éducatives et de développement. Veuillez vérifier les informations critiques pour les cas d'usage officiels.

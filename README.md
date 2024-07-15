# Gorkha_Earthquake_damage_prediction

## About
In this project, our goal is to predict the level of damage to buildings caused by the 2015 Gorkha earthquake in Nepal. The data was collected through surveys by Kathmandu Living Labs and the Central Bureau of Statistics, which works under the National Planning Commission Secretariat of Nepal. This survey is one of the largest post-disaster datasets ever collected, containing valuable information on earthquake impacts, household conditions, and socio-economic-demographic statistics.

## Objective
The specific task is to predict the ordinal variable `damage_grade`, which categorizes the extent of damage to a building into three grades:
- **Grade 1**: Represents low damage
- **Grade 2**: Represents a moderate amount of damage
- **Grade 3**: Represents almost complete destruction

## Dataset Overview
The dataset mainly consists of information on the buildings' structure and their legal ownership. Each row in the dataset represents a specific building in the region that was hit by the Gorkha earthquake.

There are 39 columns in this dataset, where the `building_id` column is a unique and random identifier. The remaining 38 features are described in the section below. Categorical variables have been obfuscated random lowercase ASCII characters. The appearance of the same character in distinct columns does not imply the same original value.

### Description

| Column | Description | Data Type |
| --- | --- | --- |
| `geo_level_1_id`, `geo_level_2_id`, `geo_level_3_id` | Geographic region in which building exists, from largest (level 1) to most specific sub-region (level 3). Possible values: level 1: 0-30, level 2: 0-1427, level 3: 0-12567. | int |
| `count_floors_pre_eq` | Number of floors in the building before the earthquake. | int |
| `age` | Age of the building in years. | int |
| `area_percentage` | Normalized area of the building footprint. | int |
| `height_percentage` | Normalized height of the building footprint. | int |
| `land_surface_condition` | Surface condition of the land where the building was built. Possible values: n, o, t. | categorical |
| `foundation_type` | Type of foundation used while building. Possible values: h, i, r, u, w. | categorical |
| `roof_type` | Type of roof used while building. Possible values: n, q, x. | categorical |
| `ground_floor_type` | Type of the ground floor. Possible values: f, m, v, x, z. | categorical |
| `other_floor_type` | Type of constructions used in higher than the ground floors (except of roof). Possible values: j, q, s, x. | categorical |
| `position` | Position of the building. Possible values: j, o, s, t. | categorical |
| `plan_configuration` | Building plan configuration. Possible values: a, c, d, f, m, n, o, q, s, u. | categorical |
| `has_superstructure_adobe_mud` | Flag variable that indicates if the superstructure was made of Adobe/Mud. | binary |
| `has_superstructure_mud_mortar_stone` | Flag variable that indicates if the superstructure was made of Mud Mortar - Stone. | binary |
| `has_superstructure_stone_flag` | Flag variable that indicates if the superstructure was made of Stone. | binary |
| `has_superstructure_cement_mortar_stone` | Flag variable that indicates if the superstructure was made of Cement Mortar - Stone. | binary |
| `has_superstructure_mud_mortar_brick` | Flag variable that indicates if the superstructure was made of Mud Mortar - Brick. | binary |
| `has_superstructure_cement_mortar_brick` | Flag variable that indicates if the superstructure was made of Cement Mortar - Brick. | binary |
| `has_superstructure_timber` | Flag variable that indicates if the superstructure was made of Timber. | binary |
| `has_superstructure_bamboo` | Flag variable that indicates if the superstructure was made of Bamboo. | binary |
| `has_superstructure_rc_non_engineered` | Flag variable that indicates if the superstructure was made of non-engineered reinforced concrete. | binary |
| `has_superstructure_rc_engineered` | Flag variable that indicates if the superstructure was made of engineered reinforced concrete. | binary |
| `has_superstructure_other` | Flag variable that indicates if the superstructure was made of any other material. | binary |
| `legal_ownership_status` | Legal ownership status of the land where building was built. Possible values: a, r, v, w. | categorical |
| `count_families` | Number of families that live in the building. | int |
| `has_secondary_use` | Flag variable that indicates if the building was used for any secondary purpose. | binary |
| `has_secondary_use_agriculture` | Flag variable that indicates if the building was used for agricultural purposes. | binary |
| `has_secondary_use_hotel` | Flag variable that indicates if the building was used as a hotel. | binary |
| `has_secondary_use_rental` | Flag variable that indicates if the building was used for rental purposes. | binary |
| `has_secondary_use_institution` | Flag variable that indicates if the building was used as a location of any institution. | binary |
| `has_secondary_use_school` | Flag variable that indicates if the building was used as a school. | binary |
| `has_secondary_use_industry` | Flag variable that indicates if the building was used for industrial purposes. | binary |
| `has_secondary_use_health_post` | Flag variable that indicates if the building was used as a health post. | binary |
| `has_secondary_use_gov_office` | Flag variable that indicates if the building was used as a government office. | binary |
| `has_secondary_use_use_police` | Flag variable that indicates if the building was used as a police station. | binary |
| `has_secondary_use_other` | Flag variable that indicates if the building was secondarily used for other purposes. | binary |

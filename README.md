# psgc-dif



The data of the Philippine Standard Geographic Code (PSGC) in the form of various data interchange formats, which are mainly comprised of these heirarchy levels: Region, Province, District, City/Mun/SubMun/SGU, and Barangay.

## Exported Files

| File Type |
| --------- |
| csv       |
| json      |
| sql       |

## Definition

| Term   | Meaning                                       |
| ------ | --------------------------------------------- |
| CMSS   | City / Municipality / Sub-Municipality / SGU  |
| SGU    | Special Government Unit or Municipal District |
| SubMun | Sub-Municipality                              |

## Modified original columns

| Original Header       | Exported Data Key     |
| --------------------- | --------------------- |
| 10-digit PSGC         | psgc_10digit          |
| Name                  | name                  |
| Correspondence Code   | correspondence_code   |
| Geographic Level      | geographic_level      |
| Old names             | old_name              |
| City Class            | city_class            |
| Income Classification | income_classification |
| Urban/Rural           | ur                    |
| 2015 Population       | popu_2015             |
| 2020 Population       | popu_2020             |
| Status                | status                |

## Added columns

| Exported Data Key     | Definition                   |
| --------------------- | ---------------------------- |
| id                    | Sequence and number          |
| is_reg                | Is Region?                   |
| is_prov               | Is Province?                 |
| is_dist               | Is District?                 |
| is_cmss               | Is any one of CMSS?          |
| is_city               | Is City?                     |
| is_municipality       | Is Municipality?             |
| is_sub_municipality   | Is Sub-Municipality?         |
| is_sgu                | Is SGU?                      |
| is_bgy                | Is Barangay?                 |
| is_urban              | Is Urban?                    |
| is_rural              | Is Rural?                    |
| is_formerly_poblacion | Is formerly Poblacion?       |
| is_capital            | Is Capital?                  |
| parent_id             | Parent ID of the current row |
| level                 | The current row depth level  |
| parent_reg            | Who is the parent Region?    |
| parent_prov           | Who is the parent Province?  |
| parent_dist           | Who is the parent District?  |
| parent_cmss           | Who is the parent CMSS?      |
| parent_bgy            | Who is the parent Barangay?  |

## Reference

- [1] Philippine Standard Geographic Code (PSGC) | Philippine Statistics Authority [Philippine Standard Geographic Code (PSGC) | Philippine Statistics Authority](https://psa.gov.ph/classification/psgc/)

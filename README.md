<!--
 ___ _            _ _    _ _    __
/ __(_)_ __  _ __| (_)__(_) |_ /_/
\__ \ | '  \| '_ \ | / _| |  _/ -_)
|___/_|_|_|_| .__/_|_\__|_|\__\___|
            |_| 
-->
![](https://platform.simplicite.io/logos/standard/logo250.png)
* * *

`Training` module definition
============================

Training module

`TrnClient` business object definition
--------------------------------------



### Fields

| Name                                                         | Type                                     | Required | Updatable | Personal | Description                                                                      |
|--------------------------------------------------------------|------------------------------------------|----------|-----------|----------|----------------------------------------------------------------------------------|
| `trnCliFirstname`                                            | char(100)                                | yes*     | yes       |          | -                                                                                |
| `trnCliLastname`                                             | char(100)                                | yes*     | yes       |          | -                                                                                |
| `trnCliMail`                                                 | email(100)                               |          | yes       |          | -                                                                                |
| `trnCliPhone`                                                | phone(100)                               |          | yes       |          | -                                                                                |
| `trnCliAddress`                                              | text(100)                                |          | yes       |          | -                                                                                |

`TrnOrder` business object definition
-------------------------------------



### Fields

| Name                                                         | Type                                     | Required | Updatable | Personal | Description                                                                      |
|--------------------------------------------------------------|------------------------------------------|----------|-----------|----------|----------------------------------------------------------------------------------|
| `trnOrdNumber`                                               | char(100)                                | yes*     | yes       |          | -                                                                                |
| `trnOrdQuantity`                                             | int(100)                                 | yes      | yes       |          | -                                                                                |
| `trnOrdDate`                                                 | datetime                                 |          | yes       |          | -                                                                                |

`TrnProduct` business object definition
---------------------------------------



### Fields

| Name                                                         | Type                                     | Required | Updatable | Personal | Description                                                                      |
|--------------------------------------------------------------|------------------------------------------|----------|-----------|----------|----------------------------------------------------------------------------------|
| `trnPrdReference`                                            | char(100)                                | yes*     | yes       |          | -                                                                                |
| `trnPrdPrice`                                                | float(100, 2)                            | yes      | yes       |          | -                                                                                |
| `trnPrdStock`                                                | int(100)                                 |          | yes       |          | -                                                                                |
| `trnPrdName`                                                 | char(100)                                |          | yes       |          | -                                                                                |
| `trnPrdDescription`                                          | text(100)                                |          | yes       |          | -                                                                                |
| `trnPrdPicture`                                              | image                                    |          | yes       |          | -                                                                                |

`TrnSupplier` business object definition
----------------------------------------

Supplier

### Fields

| Name                                                         | Type                                     | Required | Updatable | Personal | Description                                                                      |
|--------------------------------------------------------------|------------------------------------------|----------|-----------|----------|----------------------------------------------------------------------------------|
| `trnSupCode`                                                 | char(100)                                | yes*     | yes       |          | -                                                                                |
| `trnSupName`                                                 | char(100)                                |          | yes       |          | -                                                                                |
| `trnSupPhone`                                                | phone(100)                               |          | yes       |          | -                                                                                |
| `trnSupLogo`                                                 | image                                    |          | yes       |          | -                                                                                |
| `trnSupWeb`                                                  | url(100)                                 |          | yes       |          | -                                                                                |


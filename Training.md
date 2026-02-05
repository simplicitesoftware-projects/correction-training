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
| `trnOrdPrdId` link to **`TrnProduct`**                       | id                                       |          | yes       |          | -                                                                                |
| _Ref. `trnOrdPrdId.trnPrdReference`_                         | _char(100)_                              |          |           |          | -                                                                                |
| _Ref. `trnOrdPrdId.trnPrdPrice`_                             | _float(100, 2)_                          |          |           |          | -                                                                                |
| _Ref. `trnOrdPrdId.trnPrdStock`_                             | _int(100)_                               |          |           |          | -                                                                                |
| _Ref. `trnOrdPrdId.trnPrdName`_                              | _char(100)_                              |          |           |          | -                                                                                |
| _Ref. `trnOrdPrdId.trnPrdPicture`_                           | _image_                                  |          |           |          | -                                                                                |
| _Ref. `trnOrdPrdId.trnPrdSupId`_                             | _id_                                     |          |           |          | -                                                                                |
| _Ref. `trnPrdSupId.trnSupCode`_                              | _char(100)_                              |          |           |          | -                                                                                |
| `trnOrdCliId` link to **`TrnClient`**                        | id                                       |          | yes       |          | -                                                                                |
| _Ref. `trnOrdCliId.trnCliFirstname`_                         | _char(100)_                              |          |           |          | -                                                                                |
| _Ref. `trnOrdCliId.trnCliLastname`_                          | _char(100)_                              |          |           |          | -                                                                                |

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
| `trnPrdSupId` link to **`TrnSupplier`**                      | id                                       |          | yes       |          | -                                                                                |
| _Ref. `trnPrdSupId.trnSupCode`_                              | _char(100)_                              |          |           |          | -                                                                                |
| _Ref. `trnPrdSupId.trnSupName`_                              | _char(100)_                              |          |           |          | -                                                                                |

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


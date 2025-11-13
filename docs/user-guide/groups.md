# User roles and groups
G-nom users are organized into different roles to control access an editing of data. Additionally, users may join groups at the discretion of group leaders. This allows users to control data i.e. for specific project cooperatively.
!!! example "Group functionalities"

    Currently, groups are just a basic feature to organize users. Future additions to G-nom will allow for sub-groups, referred to as "Projects", whose data can be published as assembly collections and associated with relevant publications.
    


|      Role     | View data | Import data |    Alter data   |   Delete data   | Edit user roles | Create Groups | Join groups | Edit groups |       Granted by      |
|:-------------:|:---------:|:-----------:|:---------------:|:---------------:|:---------------:|:-------------:|:-----------:|:-----------:|:---------------------:|
|     Viewer    |     ✅     |      ❌      |        ❌        |        ❌        |        ❌        |       ❌       |      ✅      |      ❌      | System (default role) |
|  Contributor  |     ✅     |      ✅      |     (✅) own     |     (✅) own     |        ❌        |       ❌       |      ✅      |      ❌      |      Group Leader     |
|  Group Leader |     ✅     |      ✅      | (✅) own + group | (✅) own + group |        ✅        |       ❌       |      ✅      |      ✅      | System Administrators |
| Administrator |     ✅     |      ✅      |        ✅        |        ✅        |        ✅        |       ✅       |      ✅      |      ✅      |           -           |
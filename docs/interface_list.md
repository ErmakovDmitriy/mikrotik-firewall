interface_list rules.
1. Create interface lists as:
```
mikrotik_firewall:
  interface_list:
    - list :  "list 1 name without spaces"
      comment: "list 1 comment"
      include: "enumerated list of included interface lists separated by comma without spaces"
      exclude: "enumerated list of excluded interface lists separated by comma without spaces"
    - list :  "list 2 name without spaces"
      comment: "list 2 comment"
      include: "enumerated list of included interface lists separated by comma without spaces"
      exclude: "enumerated list of excluded interface lists separated by comma without spaces"
```
2. add members to lists like that:
```
mikrotik_firewall:
  interface_list:
    - list :  "list 1 name without spaces"
      comment: "list 1 comment"
      include: "enumerated list of included interface lists separated by comma without spaces"
      exclude: "enumerated list of excluded interface lists separated by comma without spaces"
      members:
        - interface: "interface_1_name_without_spaces"
          comment: "comment could contain spaces"
          disabled: "True or false. Could be any YAML True/False valid value"
        - interface: "interface_2_name_without_spaces"
          comment: "comment could contain spaces"
          disabled: "True or false. Could be any YAML True/False valid value"
    - list :  "list 2 name without spaces"
      comment: "list 2 comment"
      include: "enumerated list of included interface lists separated by comma without spaces"
      exclude: "enumerated list of excluded interface lists separated by comma without spaces"
```

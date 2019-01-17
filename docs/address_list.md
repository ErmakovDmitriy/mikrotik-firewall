address_list rules.
1. Create address lists as:
```
mikrotik_firewall:
  remove_old_address_list: <true|false> # Deletes ALL address lists (even which were not created by Ansible)
  address_list:
    # ALL fields must be set
    - list :  "list 1 name without spaces" # name
      comment: "list 1 comment" #comment
      disabled: <true|false> # Makes the list disabled
      address: <10.0.0.0/24> #IP v4 address (I am not sure about possibility to add IPv6 addresses with this role)

    - list :  "list 1 name without spaces" # name
      comment: "list 1 comment" #comment
      disabled: <true|false> # Makes the list disabled
      address: <10.0.1.0/24> #IP v4 address (I am not sure about possibility to add IPv6 addresses with this role)

    - list :  "list 2 name without spaces" # name
      comment: "list 2 comment" #comment
      disabled: <true|false> # Makes the list disabled
      address: <10.0.0.0/24> #IP v4 address (I am not sure about possibility to add IPv6 addresses with this role)
```

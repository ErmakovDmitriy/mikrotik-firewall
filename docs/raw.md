raw_rules:
----------
Create rules as in example below.
Unfortunately, values for keys must be quoted and valid RouterOS values
```
mikrotik_firewall:
  remove_old_raw_rules: <true|false> # If true - deletes ALL raw rules (even which were not created by Ansible)
  #List of rules. All key-value pairs are optional.
  # Rules are added to firewall in a direct list order.
  raw_rules:
    - chain:
      action:
      fragment:
      log_prefix:
      psd:
      address_list:
      hotspot:
      nth:
      random:
      address_list_timeout:
      icmp_options:
      out_bridge_port:
      src_address:
      comment:
      in_bridge_port:
      out_bridge_port_list:
      src_address_list:
      content:
      in_bridge_port_list:
      out_interface:
      src_address_type:
      copy_from:
      in_interface:
      out_interface_list:
      src_mac_address:
      disabled:
      in_interface_list:
      packet_mark:
      src_port:
      dscp:
      ingress_priority:
      packet_size:
      tcp_flags:
      dst_address:
      ipsec_policy:
      per_connection_classifier:
      tcp_mss:
      dst_address_list:
      ipv4_options:
      place_before:
      time:
      dst_address_type:
      jump_target:
      port:
      ttl:
      dst_limit:
      limit:
      priority:
      dst_port:
      log:
      protocol:
```

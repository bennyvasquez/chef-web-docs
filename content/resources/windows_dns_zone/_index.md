---
title: windows_dns_zone resource
resource: windows_dns_zone
draft: false
aliases:
- /resource_windows_dns_zone.html
menu:
  infra:
    title: windows_dns_zone
    identifier: chef_infra/cookbook_reference/resources/windows_dns_zone windows_dns_zone
    parent: chef_infra/cookbook_reference/resources
    weight: 1280
resource_reference: true
robots: null
resource_description_list:
- markdown: 'The **windows_dns_zone** resource creates an Active Directory

    Integrated DNS Zone on the local server.'
resource_new_in: '15.0'
handler_types: false
syntax_description: "The windows_dns_zone resource has the following syntax:\n\n```\
  \ ruby\nwindows_dns_zone 'name' do\n  replication_scope      String # default value:\
  \ \"Domain\"\n  server_type            String # default value: \"Domain\"\n  zone_name\
  \              String # default value: 'name' unless specified\n  action       \
  \          Symbol # defaults to :create if not specified\nend\n```"
syntax_code_block: null
syntax_properties_list:
- '`windows_dns_zone` is the resource.'
- '`name` is the name given to the resource block.'
- '`action` identifies which steps Chef Infra Client will take to bring the node into
  the desired state.'
- '`replication_scope`, `server_type`, and `zone_name` are the properties available
  to this resource.'
syntax_full_code_block: null
syntax_full_properties_list: null
syntax_shortcode: null
registry_key: false
nameless_apt_update: false
nameless_build_essential: false
resource_package_options: false
actions_list:
  :create:
    markdown: Creates and updates a DNS Zone. Default.
  :delete:
    markdown: Deletes a DNS Zone.
  :nothing:
    shortcode: resources_common_actions_nothing.md
properties_list:
- property: replication_scope
  ruby_type: String
  required: false
  default_value: '"Domain"'
  new_in: null
  description_list:
  - markdown: 'The replication scope for the zone, required if server_type set to

      ''Domain''.'
- property: server_type
  ruby_type: String
  required: false
  default_value: '"Domain"'
  new_in: null
  description_list:
  - markdown: The type of DNS server, Domain or Standalone.
- property: zone_name
  ruby_type: String
  required: false
  default_value: The resource block's name
  new_in: null
  description_list:
  - markdown: 'An optional property to set the dns zone name if it differs from the

      resource block''s name.'
properties_shortcode: null
properties_multiple_packages: false
resource_directory_recursive_directories: false
resources_common_atomic_update: false
properties_resources_common_windows_security: false
remote_file_prevent_re_downloads: false
remote_file_unc_path: false
ps_credential_helper: false
ruby_style_basics_chef_log: false
debug_recipes_chef_shell: false
template_requirements: false
resources_common_properties: true
resources_common_notification: true
resources_common_guards: true
common_resource_functionality_multiple_packages: false
resources_common_guard_interpreter: false
remote_directory_recursive_directories: false
common_resource_functionality_resources_common_windows_security: false
handler_custom: false
cookbook_file_specificity: false
unit_file_verification: false
examples_list: null

---

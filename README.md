# openstack-ansible-horizon_metadata_plugin
    cd /opt
    git clone https://github.com/dani4571/openstack-ansible-horizon_metadata_plugin.git horizon_metadata_plugin
    cd horizon_metadata_plugin/playbooks
    
edit horizon_metadata_plugin.yml set the horizon_metadata_plugin_git_branch to v1.0.0 and openstack_release to 13.2.0 (or what ever the version of OSA is)
    vars:
      horizon_metadata_plugin_git_branch: stable/mitaka
      openstack_release: 13.2.0
run the playbook
      oenstack-ansible horizon_metadata_plugin.yml

# openstack-ansible-horizon_metadata_plugin
    cd /opt
    git clone https://github.com/dani4571/openstack-ansible-horizon_metadata_plugin.git horizon_metadata_plugin
    cd horizon_metadata_plugin/playbooks
    
edit horizon_metadata_plugin.yml set the horizon_metadata_plugin_git_branch to v1.0.0 and openstack_release to 13.2.0 (or what ever the version of OSA is)
```yaml
    vars:
      horizon_metadata_plugin_git_branch: v1.0.0
      openstack_release: 13.2.0
```
run the playbook

      openstack-ansible horizon_metadata_plugin.yml

Change to new instance panel. Edit /etc/openstack_deploy/user_variables.yml 

```yaml
    horizon_launch_instance_legacy: False
    horizon_launch_instance_ng: True
```

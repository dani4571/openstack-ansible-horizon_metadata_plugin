# openstack-ansible-horizon_metadata_plugin
    cd /opt
    git clone https://github.com/michaelrice/openstack-ansible-os_horizon_metadatasearch os_horizon_metadatasearch
    cd os_horizon_metadatasearch/playbooks
    edit os_horizon_metadatasearch.yml set the horizon_metadatasearch_git_install_branch to stable/mitaka and openstack_release to 13.1.4 (or what ever the version of OSA is)
    openstack-ansible os_horizon_metadatasearch.yml

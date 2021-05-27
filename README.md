# vtools_auto_env

```yaml
Example vars:

  vars:
    pkgs:
      - git
      - virt-v2v
      - vim
      - virtio-win
      - tcpdump
      - gcc
      - virt-install
      - libvirt
      - qemu-kvm
      - platform-python-devel
    pkgs_8:
      - python3-pillow
      - python3-ovirt-engine-sdk4-4.3.4-1.el8ev.x86_64.rpm
    pkgs_9:
      - python3-ovirt-engine-sdk4-4.4.10-1.el9.x86_64.rpm
    pip_pkgs_9:
      - Pillow
    proxy_env:
      http_proxy: x.x.x.x:3128
      https_proxy: x.x.x.x:3128
    jobs_yaml: '~/jobs.yaml'
    vt_cfgs: '{{ code_root_dir }}/avocado-vt/virttest/backends/v2v/cfg/'
    tp_libvirt_cfgs: '{{ code_root_dir }}/tp-libvirt/v2v/tests/cfg/'
```
 
Usage:
1) Put your remote host's ip or hostname to the v2v_servers section of the inventory file
2) Remove the invalid fingerprint items in ~/.ssh/known_hosts file of the remote host.
3) Update the requried pkgs, e.g. ovirt-engine-sdk4, you can also add other packages you prefer to install.
4) Setup proxy server (optional). If the connection to github in unstable, you can add the proxy settings.
5) Set jobs_yaml file path (optional). If you would like all Marcos are replaced automatically based on jobs.yaml file in libvirt-ci project,
You can setup the file path of the jobs.yaml file.


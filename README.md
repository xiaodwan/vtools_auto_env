# vtools_auto_env

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
    proxy_env:
      http_proxy: x.x.x.x:3128
      https_proxy: x.x.x.x:3128
    jobs_yaml: '~/jobs.yaml'
    vt_cfgs: '{{ code_root_dir }}/avocado-vt/virttest/backends/v2v/cfg/'
    tp_libvirt_cfgs: '{{ code_root_dir }}/tp-libvirt/v2v/tests/cfg/'

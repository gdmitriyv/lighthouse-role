Role Name Lighthouse
Requirements Ubuntu linux >=20.04
Role Variables lighthouse_code_src: "https://github.com/VKCOM/lighthouse.git" lighthouse_code_src_version: d701335 lighthouse_data_dir: "/usr/share/nginx/html/lighthouse/" lighthouse_packages:

nginx
git
lighthouse_nginx_port: 8080 lighthouse_nginx_conf: "lighthouse.conf"
Dependencies clickhouse vector
Example Playbook

name: Lighthouse hosts: lighthouse gather_facts: false tags: lighthouse roles:
lighthouse
License
BSD

Author Information github.com/gdmitriyv

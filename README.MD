
Creating installation pf postgresql, with superuser val and db test_db, for example: 
ansible-playbook -i inventory/hosts install_postgres.yml --extra-vars '{"postgresql_version": "12", "postgresql_users": [{"name": "val", "password": "supersecure", "role_attr_flags": "SUPERUSER"}], "postgresql_databases": [{"name": "test_db", "owner": "val"}]}'
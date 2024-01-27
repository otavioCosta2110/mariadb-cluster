# mariadb-cluster
A simple mariadb cluster using kubernetes.

kubectl create secret generic mariadb-galera-secret --from-literal=mariadb-root-password='your-database-password-here'
FROM mysql:8.0
ENV MYSQL_ROOT_PASSWORD=ExpenseApp@1
ADD scripts/*.sql /docker-entrypoint-initdb.d
# MYSQL_DATABASE=transactions  \ we have these all setups in scripts.
# MYSQL_USER=expense \
# MYSQL_PASSWORD=ExpenseApp@1



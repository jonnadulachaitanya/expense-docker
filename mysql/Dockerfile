FROM mysql:8.0
ADD script/*.sql /docker-entrypoint-initdb.d
ENV MYSQL_ROOT_PASSWORD=ExpenseApp@1 \
  # MYSQL_DATABASE=transactions \
  # MYSQL_USER=Expense \
  # MYSQL_PASSWORD=ExpenseApp@1

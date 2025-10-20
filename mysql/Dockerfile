FROM mysql:8.0
# Below condition, As per documentation the database script should be in mention path, then it will create intial db.
ADD scripts/*.sql /docker-entrypoint-initdb.d
ENV MYSQL_ROOT_PASSWORD=ExpenseApp@1 \
  # We are commenting as below info is there in SQL file
  # MYSQL_DATABASE=transactions \
  # MYSQL_USER=Expense \
  # MYSQL_PASSWORD=ExpenseApp@1

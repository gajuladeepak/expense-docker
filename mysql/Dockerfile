FROM mysql:8.0
ENV MYSQL_ROOT_PASSWORD=ExpenseAPP@1 
ADD scripts/*.sql /docker-entrypoint-initdb.d
    # MYSQL_DATABASE=transactions \
    # MYSQL_USER=expense \
    # MYSQL_PASSWORD=ExpenseAPP@1
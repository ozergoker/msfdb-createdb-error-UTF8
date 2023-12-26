createdb: error: database creation failed: HATA:  "UTF8" dil kodlaması, "tr_TR" sunucu yereli ile eşleşmiyor
DETAIL:  Seçilen LC_TYPE ayarı, "LATIN5" dil kodlamasını gerektirir.
[+] Creating databases 'msf_test'
createdb: error: database creation failed: HATA:  "UTF8" dil kodlaması, "tr_TR" sunucu yereli ile eşleşmiyor
DETAIL:  Seçilen LC_TYPE ayarı, "LATIN5" dil kodlamasını gerektirir.
[+] Creating configuration file '/usr/share/metasploit-framework/config/database.yml'
[+] Creating initial database schema
rake aborted!
ActiveRecord::NoDatabaseError: We could not find your database: msf. Which can be found in the database configuration file located at config/database.yml.

To resolve this issue:

- Did you create the database for this app, or delete it? You may need to create your database.
- Has the database name changed? Check your database.yml config has the correct database name.

To create your database, run:

        bin/rails db:create
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/postgresql_adapter.rb:81:in `rescue in new_client'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/postgresql_adapter.rb:77:in `new_client'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/postgresql_adapter.rb:37:in `postgresql_connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/abstract/connection_pool.rb:656:in `public_send'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/abstract/connection_pool.rb:656:in `new_connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/abstract/connection_pool.rb:700:in `checkout_new_connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/abstract/connection_pool.rb:679:in `try_to_checkout_new_connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/abstract/connection_pool.rb:640:in `acquire_connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/abstract/connection_pool.rb:341:in `checkout'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/abstract/connection_pool.rb:181:in `connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/abstract/connection_handler.rb:211:in `retrieve_connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_handling.rb:313:in `retrieve_connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_handling.rb:280:in `connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/tasks/database_tasks.rb:262:in `migrate'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/railties/databases.rake:92:in `block (2 levels) in <top (required)>'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/rake-13.1.0/exe/rake:27:in `<top (required)>'

Caused by:
PG::ConnectionBad: connection to server at "::1", port 5432 failed: �L�MC�L (FATAL):  "msf" veritaban� mevcut de�il
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/pg-1.5.4/lib/pg/connection.rb:696:in `async_connect_or_reset'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/pg-1.5.4/lib/pg/connection.rb:824:in `connect_to_hosts'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/pg-1.5.4/lib/pg/connection.rb:759:in `new'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/pg-1.5.4/lib/pg.rb:63:in `connect'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/postgresql_adapter.rb:78:in `new_client'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/postgresql_adapter.rb:37:in `postgresql_connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/abstract/connection_pool.rb:656:in `public_send'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/abstract/connection_pool.rb:656:in `new_connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/abstract/connection_pool.rb:700:in `checkout_new_connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/abstract/connection_pool.rb:679:in `try_to_checkout_new_connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/abstract/connection_pool.rb:640:in `acquire_connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/abstract/connection_pool.rb:341:in `checkout'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/abstract/connection_pool.rb:181:in `connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_adapters/abstract/connection_handler.rb:211:in `retrieve_connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_handling.rb:313:in `retrieve_connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/connection_handling.rb:280:in `connection'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/tasks/database_tasks.rb:262:in `migrate'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/activerecord-7.0.8/lib/active_record/railties/databases.rake:92:in `block (2 levels) in <top (required)>'
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/rake-13.1.0/exe/rake:27:in `<top (required)>'
Tasks: TOP => db:migrate
(See full trace by running task with --trace)


postgres=# \l

                                                  List of databases
   Name    |  Owner   | Encoding | Locale Provider | Collate | Ctype | ICU Locale | ICU Rules |   Access privileges   
-----------+----------+----------+-----------------+---------+-------+------------+-----------+-----------------------
 postgres  | postgres | LATIN5   | libc            | tr_TR   | tr_TR |            |           | 
 template0 | postgres | LATIN5   | libc            | tr_TR   | tr_TR |            |           | =c/postgres          +
           |          |          |                 |         |       |            |           | postgres=CTc/postgres
 template1 | postgres | LATIN5   | libc            | tr_TR   | tr_TR |            |           | =c/postgres          +
           |          |          |                 |         |       |            |           | postgres=CTc/postgres
(3 rows)



postgres=# SET client_encoding = 'UTF8';

postgres=# UPDATE pg_database SET datcollate='en_US.UTF-8', datctype='en_US.UTF-8' WHERE datname='postgres';

postgres=# UPDATE pg_database set encoding = pg_char_to_encoding('UTF8') where datname = 'postgres' 

postgres=# UPDATE pg_database SET datcollate='en_US.UTF-8', datctype='en_US.UTF-8' WHERE datname='template0';

postgres=# UPDATE pg_database set encoding = pg_char_to_encoding('UTF8') where datname = 'template0' 

postgres=# UPDATE pg_database SET datcollate='en_US.UTF-8', datctype='en_US.UTF-8' WHERE datname='template1';

postgres=# UPDATE pg_database set encoding = pg_char_to_encoding('UTF8') where datname = 'template1' ;


msfdb reinit
[i] Database already started
[+] Dropping database user 'msf'
[+] Deleting configuration file /usr/share/metasploit-framework/config/database.yml
[+] Stopping database
[+] Starting database
[+] Creating database user 'msf'
[+] Creating databases 'msf'
[+] Creating databases 'msf_test'
[+] Creating configuration file '/usr/share/metasploit-framework/config/database.yml'
[+] Creating initial database schema


postgres=# \l
                                                       List of databases
   Name    |  Owner   | Encoding | Locale Provider |   Collate   |    Ctype    | ICU Locale | ICU Rules |   Access privileges   
-----------+----------+----------+-----------------+-------------+-------------+------------+-----------+-----------------------
 msf       | msf      | UTF8     | libc            | en_US.UTF-8 | en_US.UTF-8 |            |           | 
 msf_test  | msf      | UTF8     | libc            | en_US.UTF-8 | en_US.UTF-8 |            |           | 
 postgres  | postgres | UTF8     | libc            | en_US.UTF-8 | en_US.UTF-8 |            |           | 
 template0 | postgres | UTF8     | libc            | en_US.UTF-8 | en_US.UTF-8 |            |           | =c/postgres          +
           |          |          |                 |             |             |            |           | postgres=CTc/postgres
 template1 | postgres | UTF8     | libc            | en_US.UTF-8 | en_US.UTF-8 |            |           | =c/postgres          +
           |          |          |                 |             |             |            |           | postgres=CTc/postgres
(5 rows)


# erro-do-laravel-criacao-tabelas
Erro na criação de tabelas no laravel com phpmyadmin


PS C:\Users\Carlos Tiago\Desktop\projeto\hcode> php artisan migrate

   Illuminate\Database\QueryException 

  SQLSTATE[HY000] [1049] Unknown database 'hcode' (SQL: select * from information_schema.tables where table_schema = hcode and table_name = migrations and table_type = 'BASE TABLE')

  at C:\Users\Carlos Tiago\Desktop\projeto\hcode\vendor\laravel\framework\src\Illuminate\Database\Connection.php:703
    699▕         // If an exception occurs when attempting to run a query, we'll format the error
    700▕         // message to include the bindings with SQL, which will make this exception a
    701▕         // lot more helpful to the developer instead of just the database's errors.
    702▕         catch (Exception $e) {
  ➜ 703▕             throw new QueryException(
    704▕                 $query, $this->prepareBindings($bindings), $e
    705▕             );
    706▕         }
    707▕     }

  1   C:\Users\Carlos Tiago\Desktop\projeto\hcode\vendor\laravel\framework\src\Illuminate\Database\Connectors\Connector.php:70     
      PDOException::("SQLSTATE[HY000] [1049] Unknown database 'hcode'")

  2   C:\Users\Carlos Tiago\Desktop\projeto\hcode\vendor\laravel\framework\src\Illuminate\Database\Connectors\Connector.php:70     
      PDO::__construct("mysql:host=127.0.0.1;port=3306;dbname=hcode", "root", "", [])
PS C:\Users\Carlos Tiago\Desktop\projeto\hcode> 

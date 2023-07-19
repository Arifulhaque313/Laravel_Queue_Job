

## About Laravel Queue Job

1. This Queue Job mainly run in background and its use for consume the time 
2. First change the .env ==>  QUEUE_CONNECTION=database
3. Now, php artisan queue:table && php artisan migrate
4. php artisan make:job TestJob
5. In the app/jobs/TestJob.php you found handle function there you write the instructions 
6. i write Mail::to('asajib7654@gmial.com')->send(new TestMail); --> sending email 
7. Finally, Have to run a commnad ==> php artisan queue:work
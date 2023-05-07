TESTPROJECT/
├── app/
│   ├── Helpers/
│   │   └── ExchangeRateHelper.php
│   ├── Http/
│   │   ├── Controllers/
│   │   │   └── CommissionController.php
│   └── Services/
│       └── CommissionService.php
├── config/
├── database/
├── public/
├── resources/
│   └── view/
│       └── commissions.blade.php
├── routes/
│   └── web.php
├── storage/
├── tests/
└── vendor/



ExchangeRateHelper.php:
        This helper class fetches and caches exchange rates from the external API.

CommissionController.php: 
        This controller handles the input, processes the CSV data, and returns the results.

CommissionService.php: 
        This service class calculates the commission fees based on the provided rules.



Documentation:
    
    1) clone repository to your local machine

    2) System Execution:
        open terminal go to the project root directory and run "php artisan serve",
        This will start a development server, which you can access by opening a web browser and visiting the URL "http://localhost:8000"
    3) Go to http://127.0.0.1:8000/commissions

        there is two seperate form where you can upload csv files.   first one is connected to the exchange rate API so the result will be different from that was in the task.  all you need to do is upload cvs file and click on "Calculate Commissions"

        second form is for testing and it alwasy displays same result as was given in the task. it is using hardcoded exchage rates EUR:USD - 1:1.1497, EUR:JPY - 1:129.53.

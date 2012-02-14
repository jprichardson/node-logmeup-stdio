LogMeUp - stdio
===============

`logmeup-stdio` is a program that you can use to pipe your standard out to [LogMeUp](http://logmeup.com). You can view any log file or standard output real-time in your browser!

Install
-------

    npm install logmeup-stdio

Usage
-----

Generate a `logmeup.json` config file first:

from the console:

    $> logmeup-stdio --genconfig
    
    host: (Enter your LogMeUp installation ip address/hostname)
    port: (LogMeUp port, typically 7070)
    collection: (your collection name)
    app: (your app name)
    Generate "logmeup.json" in current directory?

    (type 'y' or 'yes' and press [ENTER] twice)
     

then from the console:

    $> yourapp | logmeup-stdio

even pipe other applications log data real-time:

    $> tail -f /var/log/mongodb.log | logmeup-stdio

    $> tail -f /var/log/apache.log | logmeup-stdio

then watch your log data real-time in your web browser:

    http://yourlogmeupserver.com:7070/:COLLECTION/:APP/

License
-------

(MIT) See [License][license] for more details.

Copyright (c) 2012 JP Richardson
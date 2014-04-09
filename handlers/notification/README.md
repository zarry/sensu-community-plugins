# Notification handlers

## mailer

The following three configuration variables must be set if you want mailer to use remote SMTP settings:

    smtp_address - defaults to "localhost"
    smtp_port - defaults to "25"
    smtp_domain - defaults to "localhost.localdomain"

## mailer_by_subscription

This mail handler works in a very similiar way to the clasic mailer with the caveat that you can define seperate mail_to values per subscription.  When the mailer runs it will check the clients subscriptions and build the mail_to field based on the default mail_to as well as clients subsciptions if corresponding values are found in the json file.

A sample mailer_by_subscription.json file was also included demonstrating how to include subscription based mailing. You can add N number of hashes for each subscription you would like a custom mail_to for.  
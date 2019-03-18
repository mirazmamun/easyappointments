Easy!Appointments++
================
This project has been forked from the foundation [EasyAppointments](https://github.com/alextselegidis/easyappointments) to customize more and add backend function for different organisation parties like:
1. Org admin
2. Org service-person
3. Org staffer

and more..

### Docker
To start Easy!Appointments using Docker in development configuration, with source files mounted into container, run:
```
docker-compose up
```

Production deployment can be made by changing required values in .env file (DB_PASSWORD, APP_URL, APP_PORT) and running:
```
docker-compose -f docker-compose.prod.yml up -d
```

Database data will be stored in named volume `easyappointments_easy-appointments-data`, and app storage (logs, cache, uploads) in `easyappointments_easy-appointments-storage`.
To find where exactly they are stored, you can run 
```
docker volume inspect easyappointments_easy-appointments-storage
```

Production containers will automatically be restarted in case of crash / server reboot. For more info, take a look into `docker-compose.prod.yml` file.

### User Feedback

Whether it is new ideas or defects, your feedback is highly appreciated and will be taken into
consideration for the following releases of the project. Share your experience and discuss your
thoughts with other users through communities. Create issues with suggestions on new features or
bug reports.

### Translate Easy!Appointments

As of version 1.0 Easy!Appointments supports translated user interface. If you want to contribute to the
translation process read the [get involved](https://github.com/alextselegidis/easyappointments/wiki/Get-Involved!)
page for additional information.

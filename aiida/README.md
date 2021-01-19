# {{ name }}
{% if description %}
{{ description }}
{% endif %}

### Introduction

This project comes with an AiiDA environment already pre-configured for you.

Get started as follows:

 1. Start a new environment (e.g. 1 CPU, 2GB memory)
 1. Open the terminal and check the status as follows:
    ```
    $ verdi status

     ✔ config dir:  /work/{{ __sanitized_project_name__ }}/repo/.aiida
     ✔ profile:     On profile {{ __sanitized_project_name__ }}
     ✔ repository:  /work/{{ __sanitized_project_name__ }}/repo/.aiida/repository/{{ __sanitized_project_name__ }}
     ✔ postgres:    Connected as aiidauser@localhost:5432
     ✔ rabbitmq:    Connected as amqp://guest:guest@127.0.0.1:5672?heartbeat=600
     ✔ daemon:      Daemon is running as PID 30575 since 2020-11-18 11:15:30
     ```
{% if archive_url %}
 1. Open the Jupyter notebook `notebooks/import_database.ipynb` for instructions on how to import the [AiiDA archive]({{ archive_url }}) selected during project creation.
{% endif %}

### Learning about AiiDA

 * The introductory [AiiDA tutorial](https://aiida.readthedocs.io/projects/aiida-core/en/latest/intro/tutorial.html), part of the [AiiDA documentation](https://aiida.readthedocs.io).
 * A [collection of historic AiiDA tutorials](https://aiida-tutorials.readthedocs.io/en/latest/) provides more extensive examples.
 * The [AiiDA web site](http://www.aiida.net) includes pointers to various other resources, such as the plugin registry, source code repository, etc.

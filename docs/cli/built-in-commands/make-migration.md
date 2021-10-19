# make:migration

Make migration -- Creates a new migration

## Options list:

```
    --name=<value>
    -n <value>
        Name of migration

    --table=<value>
    -t <value>
        Table name

    --status=<value>
    -s <value>
        Status name

    --location=<value>
    -l <value>
        Migration location. Current options are ExpressionEngine or shortname of an add-on that is currently installed. Defaults to ExpressionEngine.

    --create
    -c
        Specify command is a create command

    --update
    -u
        Specify command is an update command

```

## Examples:

### Generating a create table migration:

`php eecli.php make:migration --location=my_addon --name create_myaddon_table --create --table=addon_data`

### Generating an update table migration:

`php eecli.php make:migration --location=my_addon --name add_field_to_myaddon_table --update --table=addon_data`
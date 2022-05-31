# CarDealer DB scheme

## Model: Used_car

## Table: used_cars

- id:                       BIGINT          PK(NOTNULL, AUTO_INCREMENT, INDEX, UNIQUE)
- brand:                    VARCHAR(30)     NOTNULL, INDEX
- model:                    VARCHAR(20)     NOTNULL, INDEX
- image:                    VARCHAR(255)    NULL
- year:                     YEAR            NULL
- mileage:                  FLOAT(8,2)      NULL
- price:                    DECIMAL(8,2)    NOTNULL
- bodywork:                 VARCHAR(20)     NULL
- emissions_class:          VARCHAR(6)      NULL
- power_supply:             VARCHAR(20)     NULL
- gearbox_automatic:        TINYINT         NOTNULL DEFAULT(0)
- color:                   VARCHAR(20)     NULL
- interior_material         VARCHAR(20)     NULL
- 0_km:                     TINYINT         NOTNULL DEFAULT(0)
- previous_owners_number:   TINYINT         NOTNULL DEFAULT(1)
- kw_power:                 SMALLINT        NULL
- seats_number:             TINYINT         NULL
- doors_number:             TINYINT         NULL
- damaged_vehicle:           TINYINT         NOTNULL DEFAULT(0)
- description:                     TEXT            NULL
- note:                     TEXT            NULL
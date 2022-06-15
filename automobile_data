-- Inspect the fuel_type column

SELECT
  DISTINCT fuel_type
FROM
  [dbo].[cars_data$]

-- Inspect the length column if it aligns with the data description

SELECT
  MIN(length) AS min_length,
  MAX(length) AS max_length
FROM
   [SQL tutorial].[dbo].[cars_data$]

-- Fill in missing data

SELECT
  *
FROM
   [SQL tutorial].[dbo].[cars_data$]
WHERE 
  num_of_doors IS NULL;

UPDATE
 [dbo].[cars_data$]
SET
  num_of_doors = 'four'
WHERE
  make = 'dodge'
  AND fuel_type = 'gas'
  AND body_style = 'sedan';

UPDATE
 [dbo].[cars_data$]
SET
  num_of_doors = 'four'
WHERE
  make = 'mazda'
  AND fuel_type = 'diesel'
  AND body_style = 'sedan';

  -- identify potenial error

SELECT
  DISTINCT num_of_cylinders
FROM
  [SQL tutorial].[dbo].[cars_data$]
 
 --misspelling 

UPDATE
  [SQL tutorial].[dbo].[cars_data$]
SET
  num_of_cylinders = 'two'
WHERE
  num_of_cylinders = 'tow';

--the compression_ratio column values should range from 7 to 23.

SELECT 
MIN(compression_ratio) AS min_compression_ratio,
MAX(compression_ratio) AS max_compression_ratio
FROM 
   [SQL tutorial].[dbo].[cars_data$]
WHERE
  compression_ratio <> 70;

 SELECT
   COUNT(*) AS num_of_rows_to_delete
FROM
   [SQL tutorial].[dbo].[cars_data$]
WHERE
   compression_ratio = 70;
 
DELETE [SQL tutorial].[dbo].[cars_data$]
WHERE compression_ratio =70;

--Ensure consistency

SELECT
  DISTINCT drive_wheels
FROM 
  [SQL tutorial].[dbo].[cars_data$]

  SELECT
  DISTINCT drive_wheels,
  LENGTH(drive_wheels) AS string_length
FROM
  [SQL tutorial].[dbo].[cars_data$]

  UPDATE
  [SQL tutorial].[dbo].[cars_data$]
SET
 drive_wheels = TRIM(drive_wheels)
WHERE TRUE;

SELECT
MAX(price) AS max_price
from
  [SQL tutorial].[dbo].[cars_data$]

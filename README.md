https://gist.github.com/1b6f6b66ead53eb9fef49ad77cd0b8e6

-- This is the first query:

SELECT DISTINCT year from population_years;

-- Add your additional queries below:

select *
from population_years
where country='Gabon'
order by population desc
limit 1;

select *
from population_years
where year=2005
order by population asc
limit 10;

SELECT DISTINCT country from population_years
where population>=100
and year=2010;

select count(DISTINCT country)
from population_years
where country like '%Islands%';

select *
from population_years
where country='Indonesia'
and (year =2000 or year=2010);

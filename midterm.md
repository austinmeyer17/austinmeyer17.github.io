1.) 

SELECT county_ansi.state, county_ansi.county, county_boundaries.geometry, leso.`Item Name`, leso.quantity
  FROM county_ansi
  INNER JOIN leso
     ON county_ansi.county = leso.county
  INNER JOIN county_boundaries 
     ON county_ansi.fips = county_boundaries.fips 
     
     Where leso.`Item Name` like '%armored vehicle%'
     
     
2.) 

Loads the Polish localities (miejscowości) with their postal code and region, and fills in the
city and the region of Polish addresses from the postal code.

- Ships the list of Polish localities with their postal code, linked to the regions of Poland. The data
  comes from [GeoNames](https://www.geonames.org) (Creative Commons Attribution 4.0).
- Poland is set to *enforce cities*: the city of a Polish address is chosen from the list.
- On the contact form, typing the postal code (kod pocztowy) of a Polish address sets the city and the
  region. A postal code shared by several localities sets only the region; the city name, when it matches
  one of them (without accents and case), picks the locality.
- The action *Poland: set city from ZIP* on contacts links the Polish contacts to the city of their postal
  code and fills in the region.
- At install, the Polish contacts are linked: directly on a small database, by the scheduled action
  *Poland: link contacts to the city of their ZIP* in batches on a large one (it deactivates itself when done).
- Every form that runs the postal code rules of the contact (for example the delivery details of an AWB)
  gets the region filled in, so the shipment can be sent to Poland without looking it up by hand.

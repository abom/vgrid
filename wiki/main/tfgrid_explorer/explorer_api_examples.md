```vlang
mut tfgrid := tfgriddb.tfgrid_new() ?

entities := tfgrid.entity_list() ?
println(entities)

entity := tfgrid.entity_get_by_id(1) ?
print(entity)

twins := tfgrid.twin_list() ?
println(twins)

twin := tfgrid.twin_get_by_id(1) ?
print(twin)

nodes := tfgrid.nodes_list() ?
println(nodes)

node := tfgrid.nodes_get_by_id(1) ?
print(node)

farms := tfgrid.farms_list() ?
println(farms)

farm := tfgrid.farm_get_by_id(1) ?
print(farm)

nodes_by_resources := tfgrid.nodes_list_by_resource(1, 1, 500, 1) ?
println(nodes_by_resources)

countries := tfgrid.countries_list() ?
println(countries)

// Search for country belgium
countries_by_name_substring := tfgrid.countries_by_name_substring('elgium') ?
println(countries_by_name_substring)

country_by_id := tfgrid.country_by_id(65) ?
println(country_by_id)

cities := tfgrid.cities_list() ?
println(cities)

// Search for cities with substring "hent"
cities_by_name_substring := tfgrid.cities_by_name_substring('hent') ?
println(cities_by_name_substring)

city_by_id := tfgrid.city_by_id(65) ?
println(city_by_id)

cities_by_country_id := tfgrid.cities_by_country_id(65) ?
println(cities_by_country_id)
```

>TODO: explain more, make sure code in the vgrid repo works


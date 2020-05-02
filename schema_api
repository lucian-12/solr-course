# add a new field in solr, explicitly
# --data-binary - This posts data exactly as specified with no extra processing whatsoever.
curl -X POST -H 'Content-type:application/json' --data-binary '{
  "add-field":{
     "name":"updated_on",
     "type":"pdate",
     "indexed":true }
}' http://localhost:8983/api/cores/search_twitter/schema

# replace a field 
curl -X POST -H 'Content-type:application/json' --data-binary '{
  "replace-field":{
     "name":"updated_on",
     "type":"plong",
     "indexed":false }
}' http://localhost:8983/api/cores/search_twitter/schema

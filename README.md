# devUtils

## Linux Utils

### Check sub folders and sorty by size
du -hs * | sort -hr

### Rsync
rsync -avzh <origin> <destination>


### find directories older than 90 days & execute "du -hs --"

find  -type d -iname "*[0-9]" -mtime +90  -exec du -hs --time -- '{}' \;

find  -type d -iname "*[0-9]" -mtime +90  -exec rm -rf {} \;

## Java/Spring Utils

### Don't use config server
Put as program argument: 
--spring.cloud.config.enabled=false

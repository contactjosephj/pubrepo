# pubrepo

## Test JJ


az staticwebapp upload --name webapp1 --resource-group res_staticwebapp --source .

az staticwebapp show --name webapp1 --resource-group res_staticwebapp


swa deploy --app-location public --env production ./ --app-name webapp1 --resource-group res_staticwebapp

$token = "bf353a9a0b4ab6e2b287d4a366e555e269a2a59bbb3d2e8a9cceddec4d7bfeed02-9a69e9ff-4c0c-4d47-9e4f-435467f8595f0100229032192d10"

swa deploy ./ --app-name webapp1 --resource-group res_staticwebapp --env production  --deployment-token $token --verbose

swa deploy --app-location public --env production --deployment-token $token --verbose


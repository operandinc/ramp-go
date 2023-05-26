Unofficial Go client library for Ramp.

To re-generate:
wget https://docs.ramp.com/openapi/developer-api.json
oapi-codegen -package ramp -generate "types,client,spec" developer-api.json > ramp.gen.go
rm -f developer-api.json

One-time dependency installation for generation:
go install github.com/deepmap/oapi-codegen/cmd/oapi-codegen@latest